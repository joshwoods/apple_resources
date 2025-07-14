

- Metal
- MTLRenderStages
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a render stage from a raw value.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
init(rawValue: UInt)
```

## Parameters 

`rawValue`  

A bit field value of a render stage as an integer.

## Discussion

Use of the MTLRenderStages type’s static properties, such as mesh, vertex, or fragment instead of creating a render stage instance yourself with this initializer.

