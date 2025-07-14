

- Core Data
- NSFetchRequest
-  entityName 

Instance Property

# entityName

The name of the entity the request is configured to fetch.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var entityName: String? { get }
```

## Discussion

The entity name property is populated whenever the NSFetchRequest is created with init(entityName:) or fetchRequestWithEntityName:.

## See Also

### Managing the Fetch Request’s Entity

init()

Creates a new fetch request.

convenience init(entityName: String)

Initializes a fetch request configured with a given entity name.

var entity: NSEntityDescription?

The entity specified for the fetch request.

var includesSubentities: Bool

A Boolean value that indicates whether the fetch request includes subentities in the results.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

