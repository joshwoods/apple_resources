

- ARKit
- ARConfiguration
-  supportsFrameSemantics(\_:) 

Type Method

# supportsFrameSemantics(\_:)

Checks whether a particular feature is supported.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class func supportsFrameSemantics(_ frameSemantics: ARConfiguration.FrameSemantics) -> Bool
```

## Parameters 

`frameSemantics`  

The frame semantics for which to check device support.

## Return Value

A boolean value that indicates whether the device supports the argument frame semantics.

## Discussion

Call this function before attempting to enable a frame semantic on your app’s configuration. For example, if you call `supportsFrameSemantic(.sceneDepth)` on ARWorldTrackingConfiguration, the function returns true on devices that support the LiDAR scanner’s depth buffer.

Warning

Do not call this function on the superclass, ARConfiguration. Only configuration subclasses support frame semantics, such as those listed in `Choose your session's configuration`.

## See Also

### Enabling frame features

var frameSemantics: ARConfiguration.FrameSemantics

The set of active semantics on the frame.

struct FrameSemantics

Types of optional frame features you can enable in your app.

