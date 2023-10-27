# Entity Relationship Diagram

Reference the Creating an Entity Relationship Diagram final project guide in the course portal for more information about how to complete this deliverable.

## Create the List of Tables

- Artists
- Releases
- Tracks
- Users
- Orders
- ReleaseOrders

## Add the Entity Relationship Diagram

![Entity Relationship Diagram](./Copy%20of%20ERD_model.jpg)

### Artists

| Column Name | Type    | Description                          |
| ----------- | ------- | ------------------------------------ |
| artistID    | integer | primary key                          |
| name        | varchar | the artist or group's name           |
| genre       | varchar | the artist's identified genre        |
| location    | varchar | their self identified location       |
| imageURL    | varchar | A url for the Artist's profile image |

### Releases

| Column Name | Type          | Description                                         |
| ----------- | ------------- | --------------------------------------------------- |
| releaseID   | integer       | primary key                                         |
| title       | varchar       | the release's name                                  |
| imageURL    | varchar       | A url for the Release's image                       |
| description | text          | A description for the artist to include             |
| releasedate | date          | The release date                                    |
| price       | decimal(19,2) | The current price set by the Artist for the release |
| artistID    | integer       | foreign key - Artist Entity Pk ID                   |

### Tracks

| Column Name | Type    | Description                        |
| ----------- | ------- | ---------------------------------- |
| trackID     | integer | primary key                        |
| title       | varchar | the release's name                 |
| releaseID   | integer | foreign key - Release Entity PK ID |

### Customers

| Column Name  | Type    | Description                        |
| ------------ | ------- | ---------------------------------- |
| customerID   | integer | primary key                        |
| customername | varchar | the user's chosen profile name     |
| password     | varchar | the user's account password        |
| imageURL     | varchar | A url for the User's profile image |
| email        | varchar | The user's email                   |

### Orders

| Column Name | Type          | Description                                                                   |
| ----------- | ------------- | ----------------------------------------------------------------------------- |
| orderID     | integer       | primary key                                                                   |
| customerID  | integer       | FK - User's PK ID                                                             |
| orderDate   | date          | date of when the order was made                                               |
| totalPrice  | deicmal(19,2) | The purchase price for the release + sales tax                                |
| salesTax    | decimal(19,2) | tax to be added for the digital sale and added to the Release's current price |

### Release Orders

| Column Name    | Type          | Description                                                             |
| -------------- | ------------- | ----------------------------------------------------------------------- |
| releaseOrderID | integer       | primary key                                                             |
| orderID        | integer       | foreign key - The Order Entity's ID                                     |
| releaseID      | integer       | foreign key - The Release Entity's ID                                   |
| purchasePrice  | decimal(19,2) | foreign key - The Release Entity's current price at time of transaction |
