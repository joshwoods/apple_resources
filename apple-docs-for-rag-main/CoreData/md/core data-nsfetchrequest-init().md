

- Core Data
- NSFetchRequest
-  init() 

Initializer

# init()

Creates a new fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init()
```

## See Also

### Managing the Fetch Request’s Entity

convenience init(entityName: String)

Initializes a fetch request configured with a given entity name.

var entityName: String?

The name of the entity the request is configured to fetch.

var entity: NSEntityDescription?

The entity specified for the fetch request.

var includesSubentities: Bool

A Boolean value that indicates whether the fetch request includes subentities in the results.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

