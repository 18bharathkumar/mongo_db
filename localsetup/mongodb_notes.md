
## MongoDB Database 
MongoDB is a NoSQL database where the data is stored like in a JavaScript object.

```json
{
    "id": 1,
    "name": "Bharath Kumar"
}
```

There can also be nested data structures.

## Example

If my data collection is like this:

```json
{
    "college_name": "value",
    "college_code": "value",
    "college_photo": "value"
}
```

## Performing Operations

### Insertion

#### `insertOne` 
Used to insert a single document into a specific collection.

**Example:**

```javascript
db.collection.insertOne({
    "college_name": "value",
    "college_code": "value",
    "college_photo": "value"
})
```

Here, `collection` refers to the collection name present in the database.

#### `insertMany`
Used to insert more than one document into a collection.

**Example:**

```javascript
db.collection.insertMany([
    {
        "college_name": "value",
        "college_code": "value",
        "college_photo": "value"
    },
    {
        "college_name": "value",
        "college_code": "value",
        "college_photo": "value"
    },
    {
        "college_name": "value",
        "college_code": "value",
        "college_photo": "value"
    }
])
```
## how to filter 
**Example**
```
db.detailes.find({"college_code":"001"})
```
The above will give the document in which the college_code is 001

```
db.collection.find()
``` 
for the above we did't pass any argument in that time it will give first 20 document of perticular collection

**if we want only specific field**
```db.detailes.find({"college_code":"001"},{"college_name":1})```

Here we will get only the document which has only college_name 
<br>
1 indicates to include that field
<br>
0 indicates to exclude the field

## count method 
which will give the count of the document
**Example**
```db.detailes.find().count()```
it will work same for argument passed also
## limit method
if we want to limit the output 
**Example**
```db.detailes.find().limit(3)```
for the above i will get first 3 document only


