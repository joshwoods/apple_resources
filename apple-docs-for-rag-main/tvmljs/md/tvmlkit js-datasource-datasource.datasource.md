

- TVMLKit JS
- DataSource
-  DataSource.DataSource 

Class

# DataSource.DataSource

Methods and attributes that you use to create, modify, and access data in the data source.

tvOS 13.0+

``` source
interface DataSource
```

## Topics

### Creating the Data Source

DataSource

Creates a new data source object.

### Modifying the Data Source

insert

Inserts a new item into the array.

delete

Deletes an item from the data source array.

move

Moves an item in the data source array.

replace

Replaces an item in the data source array.

update

Updates an item in the data source array.

### Accessing Elements

item

Returns the array item at the specified index.

length

The number of items in the data source.

### Loading Elements

loadindexes

An event type that tells the data source to load its indexes.

segmentSize

The maximum number of indexes that are loaded each time the loadindexes event is triggered.

## Relationships

### Inherits From

- EventListenerObject

