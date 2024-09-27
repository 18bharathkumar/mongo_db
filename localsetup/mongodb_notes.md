
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
