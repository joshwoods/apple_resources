

- StoreKit
- SKANError
-  SKANError.Code 

Enumeration

# SKANError.Code

Constants that indicate the type of error for an ad network attribution operation.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error Codes

case adNetworkIdMissing

The ad network identifier in the ad impression doesn’t match the value in the information property list.

case impressionMissingRequiredValue

A required value is missing from a view-through ad impression.

case impressionNotFound

The system can’t find the ad impression.

case impressionTooShort

case invalidAdvertisedAppId

The App Store ID of the advertised app is invalid.

case invalidCampaignId

The campaign identifier that you provided is invalid.

case invalidConversionValue

The conversion value is invalid.

case invalidSourceAppId

The App Store ID of the app displaying the ad is invalid.

case invalidVersion

The SKAdNetwork version number is invalid.

case mismatchedSourceAppId

The source app identifier in the ad impression doesn’t match the app identifier in the source app.

case unknown

An unknown error occurred.

case unsupported

Your app attempted to use functionality that isn’t supported in the specified version.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Error handling

let SKANErrorDomain: String

A string that identifies the SKAdNetwork error domain.

struct SKANError

An error that an ad network attribution operation returns.

