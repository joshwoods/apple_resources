

- ProximityReader
- MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
-  ageAtLeastElements 

Instance Property

# ageAtLeastElements

A dictionary of values that indicate whether the document holder is at least the specified age.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
let ageAtLeastElements: [Int : Bool]
```

## Discussion

The key represents an age in years and the value is a Boolean value that indicates whether the document holder is at least that age.

