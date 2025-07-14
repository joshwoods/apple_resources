

- Metal
- MTLCommonCounter
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a common counter name from a raw value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(rawValue: String)
```

## Parameters 

`rawValue`  

The name of a common counter as a string.

## Discussion

Use of the MTLCommonCounter type’s static properties, such as timestamp, computeKernelInvocations, or totalCycles instead of creating a common counter instance yourself with this initializer.

