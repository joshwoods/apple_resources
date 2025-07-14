

- Core Data
- NSFetchRequest
-  entity 

Instance Property

# entity

The entity specified for the fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var entity: NSEntityDescription? { get set }
```

## Discussion

When an NSFetchRequest instance is created with `init()`, it is expected that the entity property will be set. If this property is not set, the fetch request fails upon execution.

## See Also

### Managing the Fetch Request’s Entity

init()

Creates a new fetch request.

convenience init(entityName: String)

Initializes a fetch request configured with a given entity name.

var entityName: String?

The name of the entity the request is configured to fetch.

var includesSubentities: Bool

A Boolean value that indicates whether the fetch request includes subentities in the results.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

