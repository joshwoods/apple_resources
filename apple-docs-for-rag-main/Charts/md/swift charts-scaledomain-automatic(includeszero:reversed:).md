

- Swift Charts
- ScaleDomain
-  automatic(includesZero:reversed:) 

Type Method

# automatic(includesZero:reversed:)

Creates a scale domain configuration that infers the scale domain from data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func automatic(
    includesZero: Bool? = nil,
    reversed: Bool? = nil
) -> AutomaticScaleDomain
```

Available when `Self` is `AutomaticScaleDomain`.

## Parameters 

`includesZero`  

Whether the scale domain should include zero (only applicable for numerical values).

`reversed`  

Whether the scale domain should be reversed (e.g., 100 … 0).

