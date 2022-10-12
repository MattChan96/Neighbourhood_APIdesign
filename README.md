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

