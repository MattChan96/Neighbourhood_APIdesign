# Neighbourhood API Design

The aim is to build a neighbourhood collaboration site with a system to track people, houses and addresses.

## Database

The database schema is split into 3 tables:

1. Person
| personID | name | age  | household | 
| ------------- | ------------- | ------------- | ------------- |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  |

2. House (addressID, personID, houseID)
| addressID | personID | houseID
| ------------- | ------------- | ------------- |
| Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  |
