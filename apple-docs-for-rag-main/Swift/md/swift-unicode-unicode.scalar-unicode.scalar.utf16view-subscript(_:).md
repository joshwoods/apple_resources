

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.UTF16View
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the code unit at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(position: Int) -> UTF16.CodeUnit { get }
```

## Parameters 

`position`  

The position of the element to access. `position` must be a valid index of the collection that is not equal to the `endIndex` property.

