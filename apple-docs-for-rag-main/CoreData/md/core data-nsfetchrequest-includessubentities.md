

- Core Data
- NSFetchRequest
-  includesSubentities 

Instance Property

# includesSubentities

A Boolean value that indicates whether the fetch request includes subentities in the results.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var includesSubentities: Bool { get set }
```

## Discussion

The value is true if the request will include all subentities of the entity for the request; otherwise it is false. The default is true.

## See Also

### Managing the Fetch Request’s Entity

init()

Creates a new fetch request.

convenience init(entityName: String)

Initializes a fetch request configured with a given entity name.

var entityName: String?

The name of the entity the request is configured to fetch.

var entity: NSEntityDescription?

The entity specified for the fetch request.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

