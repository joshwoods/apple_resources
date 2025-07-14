

- SwiftUI
- Scene
-  immersiveContentBrightness(\_:) 

Instance Method

# immersiveContentBrightness(\_:)

Sets the content brightness of an immersive space.

visionOS 1.0+

``` source
nonisolated
func immersiveContentBrightness(_ brightness: ImmersiveContentBrightness) -> some Scene
```

## Parameters 

`brightness`  

The level of content brightness that you prefer.

## Return Value

A scene that has the specified content brightness.

## Discussion

Pass one of the standard brightness levels defined in ImmersiveContentBrightness or a custom one that you create with the custom(_:) method to this scene modifier to set a preference for the content brightness in an ImmersiveSpace. The system takes the value that you set into account, but might not be able to honor a specific preference.

When you do this to create an environment that’s suitable for video playback, the standard brightness values provide good results for most use cases. To optimize further, you can create a custom brightness using a normalized value that expresses the linear brightness ratio between a standard dynamic range white video frame and the background that surrounds the player window.

Important

This modifier doesn’t affect scenes other than immersive spaces.

## See Also

### Adjusting content brightness

struct ImmersiveContentBrightness

The content brightness of an immersive space.

