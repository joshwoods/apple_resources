

- AVFoundation
- AVAsynchronousKeyValueLoading
-  load(\_:\_:\_:\_:\_:\_:\_:) 

Instance Method

# load(\_:\_:\_:\_:\_:\_:\_:)

Loads seven properties asynchronously and returns the values.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func load(
    _ propertyA: AVAsyncProperty,
    _ propertyB: AVAsyncProperty,
    _ propertyC: AVAsyncProperty,
    _ propertyD: AVAsyncProperty,
    _ propertyE: AVAsyncProperty,
    _ propertyF: AVAsyncProperty,
    _ propertyG: AVAsyncProperty
) async throws -> (A, B, C, D, E, F, G)
```

## Parameters 

`propertyA`  

A property to load.

`propertyB`  

A second property to load.

`propertyC`  

A third property to load.

`propertyD`  

A fourth property to load.

`propertyE`  

A fifth property to load.

`propertyF`  

A sixth property to load.

`propertyG`  

A seventh property to load.

## Return Value

The loaded properties in a tuple.

## Discussion

See the load(_:) method for more information.

## See Also

### Loading Property Values

func load&lt;T>(AVAsyncProperty&lt;Self, T>) async throws -> T

Loads a property asynchronously and returns the value.

func load&lt;A, B>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>) async throws -> (A, B)

Loads two properties asynchronously and returns the values.

func load&lt;A, B, C>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>) async throws -> (A, B, C)

Loads three properties asynchronously and returns the values.

func load&lt;A, B, C, D>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>) async throws -> (A, B, C, D)

Loads four properties asynchronously and returns the values.

func load&lt;A, B, C, D, E>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>, AVAsyncProperty&lt;Self, E>) async throws -> (A, B, C, D, E)

Loads five properties asynchronously and returns the values.

func load&lt;A, B, C, D, E, F>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>, AVAsyncProperty&lt;Self, E>, AVAsyncProperty&lt;Self, F>) async throws -> (A, B, C, D, E, F)

Loads six properties asynchronously and returns the values.

func load&lt;A, B, C, D, E, F, G, H>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>, AVAsyncProperty&lt;Self, E>, AVAsyncProperty&lt;Self, F>, AVAsyncProperty&lt;Self, G>, AVAsyncProperty&lt;Self, H>) async throws -> (A, B, C, D, E, F, G, H)

Loads eight properties asynchronously and returns the values.

