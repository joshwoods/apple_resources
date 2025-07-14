

- ProximityReader
- MobileDriversLicenseDisplayRequest
-  displayDriversLicense(\_:options:) 

Type Method

# displayDriversLicense(\_:options:)

A request that displays driver’s license elements onscreen.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
static func displayDriversLicense(
    _ elements: [MobileDriversLicenseDisplayRequest.Element],
    options: MobileDriversLicenseDisplayRequest.Options = .init()
) -> Self
```

Available when `Self` is `MobileDriversLicenseDisplayRequest`.

