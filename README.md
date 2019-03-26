![CF](http://i.imgur.com/7v5ASc8.png) LAB
=================================================

## Lab-06
### Author: Chris Merritt
### Links and Resources
* [PR]: http://

* [front-end] https://codesandbox.io/s/mmqry1y4qx

#### Documentation

* [swagger][]



### Setup
#### `.env` requirements`
* `3000` - assign a port number

#### Running the app
* `json-server --watch= ./data/db.json`

#### HTTP requests:
echo '{"name" : "Electronics"}' | http :3000/categories

echo '{"name": "TV", "category": "Electronics", "price" : 500}' | http :3000

echo '{"name": "TV", "category": "Electronics", "price" : 500}' | http :3000/products

echo '{"_id": 2, "name":"b",  "display_name" : "Electronics", "description" : "Electronic appliances and entertainment systems"}' | http :3000/categories

echo '{"_id": 1, "name":"Mechanical",  "display_name" : "Vehicl
es", "description" : "Car parts and stuff"}' | http :3000/categories

echo '{"_id": 2, "category":"Electronics", "name" : "Samsung", "display_name":"Samsung TV", "description" : "70 inch smart tv"}' | http :3000/products

echo '{"_id": 3, "category":"Mechanical", "name" : "Toyota", "display_name":"Toyota Prius", "description" : "Energy efficient car"}' | http :3000/products

echo '{"_id": 3, "category":"Mechanical", "name" : "Toyota", "display_name":"Toyota Prius", "description" : "Energy efficient car"}' | http :3000/products

echo '{"_id": 4, "category":"Mechanical", "name" : "Ford", "display_name":"Ford Focus", "description" : "Red car"}' | http :3000/products

http delete :3000/categories/2

http delete :3000/products/4  