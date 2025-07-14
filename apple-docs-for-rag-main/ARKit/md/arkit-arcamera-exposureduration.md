

- ARKit
- ARCamera
-  exposureDuration 

Instance Property

# exposureDuration

A value you use to effect motion blur when rendering your app’s virtual content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var exposureDuration: TimeInterval { get }
```

## Discussion

If you display an AR experience using a custom Metal renderer, use this value to determine how much motion blur to apply to your virtual content.

If ARSCNView is your renderer, SceneKit automatically applies motion blur to your virtual content. For more information, see rendersMotionBlur.

