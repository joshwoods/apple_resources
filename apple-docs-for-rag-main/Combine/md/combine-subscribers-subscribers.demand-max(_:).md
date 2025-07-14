

- Combine
- Subscribers
- Subscribers.Demand
-  max(\_:) 

Type Method

# max(\_:)

Creates a demand for the given maximum number of elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func max(_ value: Int) -> Subscribers.Demand
```

## Parameters 

`value`  

The maximum number of elements. Providing a negative value for this parameter results in a fatal error.

## Discussion

The publisher is free to send fewer than the requested maximum number of elements.

