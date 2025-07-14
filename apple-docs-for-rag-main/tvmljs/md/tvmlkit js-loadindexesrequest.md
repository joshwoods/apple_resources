

- TVMLKit JS
-  LoadIndexesRequest 

Class

# LoadIndexesRequest

A request created when the loadindexes event is triggered.

tvOS 13.0+

``` source
interface LoadIndexesRequest
```

## Topics

### Accessing Request Properties

dataSource

A reference to the data source object that originated the request.

range

The index range to load.

### Canceling Requests

cancel

Cancels the load request.

### Completing the Request

close

Signals whether or not the data fetch is successful.

## Relationships

### Inherits From

- EventListenerObject

## See Also

### Data Storage and Retrieval

Binding JSON data to TVML documents

Create full-fledged TVML documents by using data binding and queries on simplified TVML files.

XMLHttpRequest

An object used to retrieve data from a URL.

DataItem

An object used to create observable objects from JSON objects for data binding.

Storage

An object used to store key-value-pair information.

DataSource

An interface that allows the system to detect and respond to changes in your data.

