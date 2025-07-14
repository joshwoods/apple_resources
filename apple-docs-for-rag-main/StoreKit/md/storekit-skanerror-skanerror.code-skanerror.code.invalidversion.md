

- StoreKit
- SKANError
- SKANError.Code
-  SKANError.Code.invalidVersion 

Case

# SKANError.Code.invalidVersion

The SKAdNetwork version number is invalid.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
case invalidVersion
```

## Discussion

Ad networks provide an SKAdNetwork version number when preparing an ad impression, in SKStoreProductParameterAdNetworkVersion or version. Check that the version number is valid and that you follow the version-specific instructions to generate a signature. For more information about versions, see SKAdNetwork release notes.

## See Also

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

case mismatchedSourceAppId

The source app identifier in the ad impression doesn’t match the app identifier in the source app.

case unknown

An unknown error occurred.

case unsupported

Your app attempted to use functionality that isn’t supported in the specified version.

