# Neighbourhood API Design

The aim is to build a neighbourhood collaboration site with a system to track people, houses and addresses.

## Database

The implemented type of database is SQL due to the data being structured and facilitating the maintenance of data integrity. The schema is split into 3 tables:

1. Person

| personID | name | age  | household | 
| ------------- | ------------- | ------------- | ------------- |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  |

2. House

| addressID | personID | houseID |
| ------------- | ------------- | ------------- |
| Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  |

3. Address

| addressID | street | postal code |
| ------------- | ------------- | ------------- |
| Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  |

## API

Our API should be capable of handling both **GET** & **POST** requests.

### GET

**GET** requests should be a able to retrieve:
  - House data via the route `/home/id`
  - Person data (with specified queries) via the route `/people?age>0&age<100&household=x&limit=y`

**GET** responses should include:
  - House data with the keys id, owner & address: `{
    id:
    owner:
    address:
}`
  - Person data with the keys id, name, age, household: `[
    {
        id:
        name:
        age:
        household:
    },
    ...
]`

### POST

**POST** requests should be a able to add:
  - House data via the route `/houses`
  - Address data via the route `/addresses`
  - Person data via the route `/people`  


