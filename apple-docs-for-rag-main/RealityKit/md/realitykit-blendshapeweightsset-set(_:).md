

- RealityKit
- BlendShapeWeightsSet
-  set(\_:) 

Instance Method

# set(\_:)

Updates a blend shape weights data instance in the set based on its name. If blend shape weights data with this ID does not exist, does nothing.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@discardableResult
mutating func set(_ newValue: BlendShapeWeightsSet.Element) -> BlendShapeWeightsSet.Element?
```

## Parameters 

`newValue`  

The blend shape weights data to store.

## Return Value

The previous pose value, if named pose exists. nil otherwise.

