

- Create ML Components
- DateFeatureExtractor
-  init(features:calendar:) 

Initializer

# init(features:calendar:)

Creates a date feature extractor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    features: DateFeatures,
    calendar: Calendar = Calendar.current
)
```

## Parameters 

`features`  

The date and time features.

`calendar`  

The calendar to use, defaults to `Calendar.current`.

