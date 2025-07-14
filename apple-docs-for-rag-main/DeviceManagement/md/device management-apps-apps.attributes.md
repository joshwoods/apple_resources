

- Device Management
- Apps
-  Apps.Attributes 

Object

# Apps.Attributes

The attributes for an apps resource.

Device Assignment ServicesVPP License Management

``` source
object Apps.Attributes
```

## Properties

`artistName`

`string`

 (Required) 

The name of the artist for this content.

`artwork`

Artwork

 (Required) 

The artwork for this content.

`bundleId`

`string`

 (Required) 

The bundle identifier string associated with this content.

`contentRatingsBySystem`

Apps.Attributes.ContentRatingsBySystem

 (Required) 

Rating and advisory information (may be multiple per item).

`description`

DescriptionAttribute

The description for the content.

`deviceFamilies`

`[string]`

 (Required) 

The device families the app supports.

`externalVersionId`

`integer`

 (Required) 

The external version identifier.

`fileSizeByDevice`

Apps.Attributes.FileSizeByDevice

**(Extended)** A list of app file sizes by device.

`genreDisplayName`

`string`

The localized genre name for display purposes.

`hasEula`

`boolean`

 (Required) 

A Boolean indicating whether the resource has a EULA.

`isB2BCustomApp`

`boolean`

 (Required) 

A Boolean indicating whether the app is a B2B Custom App.

`isFirstPartyHideableApp`

`boolean`

 (Required) 

A Boolean indicating whether the app is a hideable first-party app.

`isIOSBinaryMacOSCompatible`

`boolean`

 (Required) 

`isVisionOSCompatible`

`boolean`

`isVppDeviceBasedLicensingEnabled`

`boolean`

 (Required) 

A Boolean indicating whether VPP device-based licensing is enabled.

`languageList`

`[string]`

**(Extended)** The language list for the app.

`latestVersionInfo`

Apps.Attributes.LatestVersionInfo

**(Extended)** A version info map for the latest version of the app.

`macRequiredCapabilities`

`string`

`minimumMacOSVersion`

`string`

`minimumOSVersion`

`string`

 (Required) 

The minimum OS version required for an app.

`minimumVisionOSVersion`

`string`

`name`

`string`

 (Required) 

The (potentially) censored name of the content.

`offers`

`[`Apps.Attributes.Offers`]`

 (Required) 

A map of offer and asset information for the associated content.

`privacyPolicyUrl`

`string`

**(Extended)** A string for the privacy policy for this app.

`requiredCapabilities`

`string`

The required capabilities for this app, if any.

`requiredCapabilitiesForRealityDevice`

`string`

`requirementsByDeviceFamily`

Apps.Attributes.RequirementsByDeviceFamily

**(Extended)** A map of requirements and supported devices by device family.

`screenshotsByType`

Apps.Attributes.ScreenshotsByType

**(Extended)** A map of artworks representing screenshots for the app by type string.

`seller`

`string`

Seller for the app.

`subtitle`

`string`

Subtitle of the app.

`supportsDeviceSharing`

`boolean`

A Boolean indicating whether multiple users can share this app on the same device.

`supportURLForLanguage`

`string`

**(Extended)** Support URL for language for the app.

`taxExclusivePrices`

`[`Apps.Attributes.TaxExclusivePrices`]`

**(Personalized)** Tax-exclusive prices for this salable.

`taxRate`

`number`

**(Personalized)** Tax rate for this salable for the current account.

`url`

`string`

 (Required) 

A canonical URL to the content that may be used for sharing or linking to the content externally.

`userRating`

Apps.Attributes.UserRating

 (Required) 

User rating information for the content. Also shows current version information for apps.

`usesClassKit`

`boolean`

A Boolean indicating whether this app uses the ClassKit deployment framework.

`versionHistory`

`[`Apps.Attributes.VersionHistory`]`

**(Extended)** Version history for the app.

`watchBundleId`

`string`

The watch bundle identifier string associated with the app.

`websiteUrl`

`string`

**(Extended)** Website URL for the app.

## Topics

### Related Objects

object Apps.Attributes.ContentRatingsBySystem

object Apps.Attributes.FileSizeByDevice

object Apps.Attributes.LatestVersionInfo

object Apps.Attributes.Offers

object Apps.Attributes.RequirementsByDeviceFamily

object Apps.Attributes.ScreenshotsByType

object Apps.Attributes.TaxExclusivePrices

object Apps.Attributes.UserRating

object Apps.Attributes.VersionHistory

## See Also

### Related Objects

object Apps.Relationships

The relationships for an apps resource.

