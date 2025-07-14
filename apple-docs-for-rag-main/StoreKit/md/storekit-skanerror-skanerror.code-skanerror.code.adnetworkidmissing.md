

- StoreKit
- SKANError
- SKANError.Code
-  SKANError.Code.adNetworkIdMissing 

Case

# SKANError.Code.adNetworkIdMissing

The ad network identifier in the ad impression doesn’t match the value in the information property list.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
case adNetworkIdMissing
```

## Discussion

The value you specify for your ad network identifier in your ad impresion must match the value in the `Info.plist`. \`\`An app that participates in ad campaigns by displaying ads must include the ad network identifiers in its `Info.plist`. For more information, see Configuring a source app.

## See Also

### Error Codes

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

