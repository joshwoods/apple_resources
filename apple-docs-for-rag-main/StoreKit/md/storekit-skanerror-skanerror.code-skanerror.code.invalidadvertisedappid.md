

- StoreKit
- SKANError
- SKANError.Code
-  SKANError.Code.invalidAdvertisedAppId 

Case

# SKANError.Code.invalidAdvertisedAppId

The App Store ID of the advertised app is invalid.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
case invalidAdvertisedAppId
```

## Discussion

Ad networks provide an advertised app identifier when signing an ad impression. If you’re providing a StoreKit-rendered ad, check that the value you set for SKStoreProductParameterITunesItemIdentifier in loadProduct(withParameters:completionBlock:) is a valid app identifer. If you’re providing a view-through ad, check the value of advertisedAppStoreItemIdentifier.

## See Also

### Error Codes

case adNetworkIdMissing

The ad network identifier in the ad impression doesn’t match the value in the information property list.

case impressionMissingRequiredValue

A required value is missing from a view-through ad impression.

case impressionNotFound

The system can’t find the ad impression.

case impressionTooShort

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

