

- StoreKit
- SKANError
- SKANError.Code
-  SKANError.Code.invalidConversionValue 

Case

# SKANError.Code.invalidConversionValue

The conversion value is invalid.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
case invalidConversionValue
```

## Discussion

Apps provide a conversion value when calling updatePostbackConversionValue(_:completionHandler:) or updateConversionValue(_:). Check that the conversion value you provide is within the allowed range.

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

