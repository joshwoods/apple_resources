

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.UTF8View
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the code unit at the specified position.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
subscript(position: Int) -> UTF8.CodeUnit { get }
```

## Parameters 

`position`  

The position of the element to access. `position` must be a valid index of the collection that is not equal to the `endIndex` property.

