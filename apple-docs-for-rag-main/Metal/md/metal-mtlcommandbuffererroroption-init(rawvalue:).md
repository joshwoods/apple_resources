

- Metal
- MTLCommandBufferErrorOption
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a set of error options from a raw integer value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(rawValue: UInt)
```

## Parameters 

`rawValue`  

The set of flags to use.

## Discussion

Use the MTLCommandBufferErrorOption structure’s type properties, such as encoderExecutionStatus, instead of this initializer.

