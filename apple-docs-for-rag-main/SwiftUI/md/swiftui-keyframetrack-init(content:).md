

- SwiftUI
- KeyframeTrack
-  init(content:) 

Initializer

# init(content:)

Creates an instance that animates the entire value from the root of the key path.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(@KeyframeTrackContentBuilder content: () -> Content) where Root == Value
```

## See Also

### Creating a keyframe track

init(WritableKeyPath&lt;Root, Value>, content: () -> Content)

Creates an instance that animates the property of the root value at the given key path.

