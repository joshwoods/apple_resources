

- Core Data
- NSBatchInsertRequest
-  managedObjectHandler 

Instance Property

# managedObjectHandler

A closure that provides a managed object for your app to insert data into.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var managedObjectHandler: ((NSManagedObject) -> Bool)? { get set }
```

## See Also

### Configuring a Request

var dictionaryHandler: ((NSMutableDictionary) -> Bool)?

A closure that provides a dictionary for your app to insert data into.

var entity: NSEntityDescription?

The managed entity to insert data into.

var entityName: String

The name of the managed entity to insert data into.

var objectsToInsert: [[String : Any]]?

An array of dictionaries that represents the objects to insert with the keys as attribute names and their assigned values.

var resultType: NSBatchInsertRequestResultType

The type of result that Core Data returns from this request.

