

- Create ML Components
- DateFeatureExtractor
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Extracts features of a particular date.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func applied(
    to date: Date,
    eventHandler: EventHandler? = nil
) -> [Scalar]
```

## Parameters 

`date`  

The date.

`eventHandler`  

An event handler.

## Return Value

An array of feature values.

