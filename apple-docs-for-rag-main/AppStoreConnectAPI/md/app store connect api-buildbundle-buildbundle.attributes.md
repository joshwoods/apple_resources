

- App Store Connect API
- BuildBundle
-  BuildBundle.Attributes 

Object

# BuildBundle.Attributes

The attributes that describe a Build Bundles resource.

App Store Connect API 1.6+

``` source
object BuildBundle.Attributes
```

## Properties

`bundleId`

`string`

The bundle ID of the build bundle.

`bundleType`

`string`

The type of the build bundle.

Possible Values: `APP, APP_CLIP`

`deviceProtocols`

`[string]`

The protocols that the app uses to communicate with external accessory hardware. For more information, see UISupportedExternalAccessoryProtocols.

`dSYMUrl`

`uri`

The URL to the symbolication file for the app or App Clip.

`entitlements`

BuildBundle.Attributes.Entitlements

Entitlement information for your app or App Clip.

`fileName`

`string`

The name of the build bundle.

`hasOnDemandResources`

`boolean`

A Boolean value that indicates whether the build bundle contains on-demand resources.

`hasPrerenderedIcon`

`boolean`

A Boolean value that indicates whether the build bundle contains a pre-rendered app icon.

`hasSirikit`

`boolean`

A Boolean value that indicates whether the build bundle contains an app or App Clip that allows users to interact with it through voice, intelligent suggestions, and personalized workflows.

`includesSymbols`

`boolean`

A Boolean value that indicates whether the build bundle includes symbol information for debugging and crash reports.

`isIosBuildMacAppStoreCompatible`

`boolean`

A Boolean value that indicates whether an iOS app included in the build bundle is included on the Mac App Store.

`locales`

`[string]`

The specified locale. Refer to BetaAppLocalizationCreateRequest.Data.Attributes for possible values.

`platformBuild`

`string`

The build number of the OS you used to build the app or App Clip.

`requiredCapabilities`

`[string]`

An array of capabilities that your app or App Clip requires.

`sdkBuild`

`string`

A string that identifies the SDK you used to build your app or App Clip.

`supportedArchitectures`

`[string]`

An array of supported CPU architectures that your app or App Clip supports.

`usesLocationServices`

`boolean`

A Boolean value that indicates whether the app or App Clip included in the build bundle uses location services.

## Topics

### Objects

object BuildBundle.Attributes.Entitlements

Entitlement information for your app or App Clip.

## See Also

### Objects

object BuildBundle.Relationships

The relationships of the Build Bundles resource you included in the request and those on which you can operate.

