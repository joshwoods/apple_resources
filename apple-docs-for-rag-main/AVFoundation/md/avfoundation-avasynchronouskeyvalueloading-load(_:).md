

- AVFoundation
- AVAsynchronousKeyValueLoading
-  load(\_:) 

Instance Method

# load(\_:)

Loads a property asynchronously and returns the value.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func load(_ property: AVAsyncProperty) async throws -> T
```

## Parameters 

`property`  

A property to load.

## Return Value

The loaded property value.

## Mentioned in 

Loading media data asynchronously

## Discussion

Call this method from an asynchronous context to load the value of one or more media properties. The method returns a single result if you load one property value, and returns a tuple if you load multiple properties (up to eight) at the same time.

To load a property, pass one or more AVAsyncProperty constants to this method as shown below.

```
// Load an asset's list of tracks.
let tracks = try await asset.load(.tracks)

// Load an asset's suitability for playback and export.
let (isPlayable, isExportable) = try await asset.load(.isPlayable, .isExportable)
```

## See Also

### Loading Property Values

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

func load&lt;A, B, C, D, E, F, G>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>, AVAsyncProperty&lt;Self, E>, AVAsyncProperty&lt;Self, F>, AVAsyncProperty&lt;Self, G>) async throws -> (A, B, C, D, E, F, G)

Loads seven properties asynchronously and returns the values.

func load&lt;A, B, C, D, E, F, G, H>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>, AVAsyncProperty&lt;Self, E>, AVAsyncProperty&lt;Self, F>, AVAsyncProperty&lt;Self, G>, AVAsyncProperty&lt;Self, H>) async throws -> (A, B, C, D, E, F, G, H)

Loads eight properties asynchronously and returns the values.

