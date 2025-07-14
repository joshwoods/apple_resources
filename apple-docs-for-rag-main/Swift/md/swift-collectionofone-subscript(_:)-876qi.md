

- Swift
- CollectionOfOne
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(position: Int) -> Element { get set }
```

## Parameters 

`position`  

The position of the element to access. The only valid position in a `CollectionOfOne` instance is `0`.

