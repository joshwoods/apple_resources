

- Create ML Components
- SlidingWindows
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the window at the specified position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
subscript(position: Int) -> MLShapedArray { get }
```

## Parameters 

`position`  

The position of the window to access. `position` must be a valid index of the collection that is not equal to the `endIndex` property.

