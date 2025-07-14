

- GameplayKit
- GKComponentSystem
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the component at the specified index in the system’s list of components.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
subscript(idx: Int) -> ComponentType { get }
```

## Parameters 

`idx`  

A valid index to the components array.

## Return Value

The component at the specified index in the components array.

## Discussion

This method is equivalent to accessing objects by index in the components array, but allows access using subscript syntax on the component system itself.

