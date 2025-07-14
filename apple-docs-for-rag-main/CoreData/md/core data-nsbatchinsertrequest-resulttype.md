

- Core Data
- NSBatchInsertRequest
-  resultType 

Instance Property

# resultType

The type of result that Core Data returns from this request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var resultType: NSBatchInsertRequestResultType { get set }
```

## Discussion

The default is NSBatchInsertRequestResultType.statusOnly.

## See Also

### Configuring a Request

var dictionaryHandler: ((NSMutableDictionary) -> Bool)?

A closure that provides a dictionary for your app to insert data into.

var entity: NSEntityDescription?

The managed entity to insert data into.

var entityName: String

The name of the managed entity to insert data into.

var managedObjectHandler: ((NSManagedObject) -> Bool)?

A closure that provides a managed object for your app to insert data into.

var objectsToInsert: [[String : Any]]?

An array of dictionaries that represents the objects to insert with the keys as attribute names and their assigned values.

