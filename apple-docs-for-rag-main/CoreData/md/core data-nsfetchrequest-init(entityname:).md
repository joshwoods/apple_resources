

- Core Data
- NSFetchRequest
-  init(entityName:) 

Initializer

# init(entityName:)

Initializes a fetch request configured with a given entity name.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
convenience init(entityName: String)
```

## Parameters 

`entityName`  

The name of the entity to fetch.

## Return Value

A fetch request configured to fetch using the entity named `entityName`.

## Discussion

This method provides a convenient way to configure the entity for a fetch request without having to retrieve an NSEntityDescription object. When the fetch is executed, the request uses the managed object context to find the entity with the given name. The model associated with the context’s persistent store coordinator must contain an entity named `entityName`.

## See Also

### Managing the Fetch Request’s Entity

init()

Creates a new fetch request.

var entityName: String?

The name of the entity the request is configured to fetch.

var entity: NSEntityDescription?

The entity specified for the fetch request.

var includesSubentities: Bool

A Boolean value that indicates whether the fetch request includes subentities in the results.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

