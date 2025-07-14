

- RealityKit
- SkeletalPoseSet
-  set(\_:) 

Instance Method

# set(\_:)

Updates a pose in the set based on its name. If pose with this ID does not exist, does nothing.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@discardableResult
mutating func set(_ newValue: SkeletalPoseSet.Element) -> SkeletalPoseSet.Element?
```

## Parameters 

`newValue`  

The pose to store.

## Return Value

The previous pose value, if named pose exists

