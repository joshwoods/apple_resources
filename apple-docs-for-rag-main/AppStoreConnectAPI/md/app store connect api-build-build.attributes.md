

- App Store Connect API
- Build
-  Build.Attributes 

Object

# Build.Attributes

Attributes that describe a Builds resource.

App Store Connect API 1.0+

``` source
object Build.Attributes
```

## Properties

`expired`

`boolean`

A Boolean value that indicates if the build has expired. An expired build is unavailable for testing.

`iconAssetToken`

ImageAsset

The icon of the uploaded build.

`minOsVersion`

`string`

The minimum operating system version needed to test a build.

`processingState`

`string`

The processing state of the build indicating that it is not yet available for testing.

Possible Values: `PROCESSING, FAILED, INVALID, VALID`

`version`

`string`

The version number of the uploaded build.

`usesNonExemptEncryption`

`boolean`

A Boolean value that indicates whether the build uses non-exempt encryption.

`uploadedDate`

`date-time`

The date and time the build was uploaded to App Store Connect.

`expirationDate`

`date-time`

The date and time the build will auto-expire and no longer be available for testing.

`buildAudienceType`

BuildAudienceType

`computedMinMacOsVersion`

`string`

`lsMinimumSystemVersion`

`string`

## Topics

### Types

type BuildAudienceType

A string that represents the App Store Connect audience for a build.

## See Also

### Related Documentation

Builds

Manage builds for testers and submit builds for review.

### Attributes and Relationships

object Build.Relationships

The relationships you included in the request and those on which you can operate.

