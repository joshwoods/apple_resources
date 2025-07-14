

- Metal
- MTLCommonCounterSet
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a common counter set name from a raw value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(rawValue: String)
```

## Parameters 

`rawValue`  

The name of a counter set as a string.

## Discussion

Use one of the MTLCommonCounterSet type’s static properties, such as timestamp, stageUtilization, and statistic instead of creating a common counter set instance yourself with this initializer.

