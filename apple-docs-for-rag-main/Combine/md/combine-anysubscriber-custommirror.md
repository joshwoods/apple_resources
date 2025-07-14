

- Combine
- AnySubscriber
-  customMirror 

Instance Property

# customMirror

The custom mirror for this instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var customMirror: Mirror { get }
```

## Discussion

If this type has value semantics, the mirror should be unaffected by subsequent mutations of the instance.

## See Also

### Inspecting Subscriber Properties

let combineIdentifier: CombineIdentifier

A unique identifier for identifying publisher streams.

var description: String

A textual representation of this instance.

var playgroundDescription: Any

A custom playground description for this instance.

