

- RealityKit
- SkeletalPose
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a pose transformation using the index of the joint name.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
subscript(joint: String) -> Transform? { get set }
```

## Parameters 

`joint`  

The joint name of transformation to access.

## Overview

Note

Setting a joint to `nil` has no effect.

