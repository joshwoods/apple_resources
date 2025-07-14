

- StoreKit
- SKANError
- SKANError.Code
-  SKANError.Code.invalidSourceAppId 

Case

# SKANError.Code.invalidSourceAppId

The App Store ID of the app displaying the ad is invalid.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
case invalidSourceAppId
```

## Discussion

Check that the value you provide for SKStoreProductParameterAdNetworkSourceAppStoreIdentifier or sourceAppStoreItemIdentifier is correct and matches the App Store ID of the app that’s displaying the ad.

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

case invalidVersion

The SKAdNetwork version number is invalid.

case mismatchedSourceAppId

The source app identifier in the ad impression doesn’t match the app identifier in the source app.

case unknown

An unknown error occurred.

case unsupported

Your app attempted to use functionality that isn’t supported in the specified version.

