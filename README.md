# Cloud-Computing
Certainly! Here's a basic documentation for your Express.js application:

---

# Location API Documentation

## Overview

The Location API provides information about different locations, including details such as city, category, rating, price, and name. The data is stored in a JSON file named `data.json`.

## Base URL

```
http://localhost:3000
```

## Endpoints

### 1. Get All Locations

#### Endpoint

```
GET /location
```

#### Description

Retrieve information about all locations.

#### Response

```json
[
  {
    "city": "City1",
    "category": "Category1",
    "rating": 4,
    "price": 50,
    "name": "Location1"
  },
  // ... (more locations)
]
```

### 2. Get Locations by City

#### Endpoint

```
GET /location/city=:city
```

#### Parameters

- `city` (string): The name of the city.

#### Description

Retrieve locations based on the specified city.

#### Response

```json
[
  {
    "city": "City1",
    "category": "Category1",
    "rating": 4,
    "price": 50,
    "name": "Location1"
  },
  // ... (more locations)
]
```

### 3. Get Locations by Category

#### Endpoint

```
GET /location/category=:category
```

#### Parameters

- `category` (string): The category of the location.

#### Description

Retrieve locations based on the specified category.

#### Response

```json
[
  {
    "city": "City1",
    "category": "Category1",
    "rating": 4,
    "price": 50,
    "name": "Location1"
  },
  // ... (more locations)
]
```

### 4. Get Locations by Rating

#### Endpoint

```
GET /location/rating=:rating
```

#### Parameters

- `rating` (number): The rating of the location.

#### Description

Retrieve locations based on the specified rating.

#### Response

```json
[
  {
    "city": "City1",
    "category": "Category1",
    "rating": 4,
    "price": 50,
    "name": "Location1"
  },
  // ... (more locations)
]
```

### 5. Get Locations by Price

#### Endpoint

```
GET /location/price=:price
```

#### Parameters

- `price` (number): The price of the location.

#### Description

Retrieve locations based on the specified price.

#### Response

```json
[
  {
    "city": "City1",
    "category": "Category1",
    "rating": 4,
    "price": 50,
    "name": "Location1"
  },
  // ... (more locations)
]
```

### 6. Get Locations by Name

#### Endpoint

```
GET /location/name=:name
```

#### Parameters

- `name` (string): The name of the location.

#### Description

Retrieve locations based on the specified name.

#### Response

```json
[
  {
    "city": "City1",
    "category": "Category1",
    "rating": 4,
    "price": 50,
    "name": "Location1"
  }
]
```

### 7. Get Locations by City and Rating

#### Endpoint

```
GET /location/city=:city&rating=:rating
```

#### Parameters

- `city` (string): The name of the city.
- `rating` (number): The rating of the location.

#### Description

Retrieve locations based on the specified city and rating.

#### Response

```json
[
  {
    "city": "City1",
    "category": "Category1",
    "rating": 4,
    "price": 50,
    "name": "Location1"
  }
]
```

### 8. Get Locations by City and Category

#### Endpoint

```
GET /location/city=:city&category=:category
```

#### Parameters

- `city` (string): The name of the city.
- `category` (string): The category of the location.

#### Description

Retrieve locations based on the specified city and category.

#### Response

```json
[
  {
    "city": "City1",
    "category": "Category1",
    "rating": 4,
    "price": 50,
    "name": "Location1"
  }
]
```

## Running the Server

To run the server, execute the following command:

```bash
node server.js
```

The server will be running on port 3000, and you can access the API using the specified endpoints.

## RESTful API
## Get All Locations:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/location
Explanation: Returns data for all locations.
Search Locations:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/location/search?q=<searchTerm>
Explanation: Searches for locations based on the provided query parameter q, which can be a name, city, or category.
Get Locations by City:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/location/city=<city>
Explanation: Returns data for all locations in the specified city.
Get Locations by Category:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/location/category=<category>
Explanation: Returns data for all locations in the specified category.
Get Locations by Rating:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/location/rating=<rating>
Explanation: Returns data for all locations with the specified rating.
Get Locations by Price:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/location/price=<price>
Explanation: Returns data for all locations with the specified price.
Get Locations by Name:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/location/name=<name>
Explanation: Returns data for the location with the specified name.
Get Locations by City and Rating:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/location/city=<city>&rating=<rating>
Explanation: Returns data for all locations in the specified city with the specified rating.
Get Recommended Locations for a City (Rating between 4.5 and 5):

## Get Recommendations for All Cities with Ratings Between 4.4 and 5:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/recommendations/cities/rating
Explanation: Returns recommendations for all cities where the rating is between 4.4 and 5.
Get Recommendations for Jakarta:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/recommendations/cities/Depok
Explanation: Returns recommendations for Jakarta where the rating is between 4.4 and 5.
Get Recommendations for Bogor:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/recommendations/cities/Bogor
Explanation: Returns recommendations for Bogor where the rating is between 4.4 and 5.
Get Recommendations for Depok:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/recommendations/cities/Depok
Explanation: Returns recommendations for Depok where the rating is between 4.4 and 5.
Get Recommendations for Tangerang:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/recommendations/cities/Tangerang
Explanation: Returns recommendations for Tangerang where the rating is between 4.4 and 5.
Get Recommendations for Bekasi:

https://lokis-app-tourism-ghggrfpakq-uc.a.run.app/recommendations/cities/Bekasi
Explanation: Returns recommendations for Bekasi where the rating is between 4.4 and 5
