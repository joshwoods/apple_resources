

- Create ML Components
- SlidingWindows
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous range of windows.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
subscript(bounds: Range) -> Slice> { get }
```

## Parameters 

`bounds`  

A range of valid indices in the classification distribution.

