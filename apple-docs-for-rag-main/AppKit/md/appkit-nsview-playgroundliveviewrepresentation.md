

- AppKit
- NSView
-  playgroundLiveViewRepresentation 

Instance Property

# playgroundLiveViewRepresentation

A custom `PlaygroundLiveViewRepresentation` for this instance.

macOS

``` source
@MainActor @preconcurrency
var playgroundLiveViewRepresentation: PlaygroundLiveViewRepresentation { get }
```

## Discussion

The value of this property can but does not need to be the same every time; PlaygroundLiveViewables may choose to create a new view or view controller every time.

See Also

`PlaygroundLiveViewRepresentation`

