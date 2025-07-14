

- ProximityReader
- MobileNationalIDCardDataRequest
- MobileNationalIDCardDataRequest.Response
- MobileNationalIDCardDataRequest.Response.DocumentElements
-  ageAtLeastElements 

Instance Property

# ageAtLeastElements

A dictionary of values that indicate whether the document holder is at least the specified age.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
let ageAtLeastElements: [Int : Bool]
```

## Discussion

The key represents an age in years and the value is a Boolean value that indicates whether the document holder is at least that age.

