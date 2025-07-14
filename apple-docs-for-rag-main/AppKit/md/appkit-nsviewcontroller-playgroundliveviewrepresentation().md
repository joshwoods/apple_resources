

- AppKit
- NSViewController
-  playgroundLiveViewRepresentation() 

Instance Method

# playgroundLiveViewRepresentation()

Returns the `XCPlaygroundLiveViewRepresentation` for the receiver.

macOS

``` source
@MainActor @preconcurrency
func playgroundLiveViewRepresentation() -> XCPlaygroundLiveViewRepresentation
```

## Discussion

The value returned from this method can but does not need to be the same every time; XCPlaygroundLiveViewables may choose to create a new view or view controller every time.

See Also

`XCPlaygroundLiveViewRepresentation`

