

- Bundle Resources
- Information Property List
-  BAInitialDownloadRestrictions 

Property List Key

# BAInitialDownloadRestrictions

The restrictions that apply to the set of assets that download immediately after app installation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 18.4+visionOS 2.4+

## Details 

Type  

object

## Discussion

This key is required to use Background Assets.

## Topics

### Initial download restrictions

BADownloadAllowance

The combined, maximum size of the initial, non-essential asset download files.

BADownloadDomainAllowList

The permitted list of domains the extension can use when scheduling the initial set of asset downloads.

BAEssentialDownloadAllowance

The combined, maximum size of the essential asset download files.

## See Also

### Background downloads

BAMaxInstallSize

The combined, maximum size, in bytes, of the non-essential assets that download immediately after app installation.

BAManifestURL

The location URL of the app’s manifest file that contains the names and sizes of assets.

BAEssentialMaxInstallSize

The combined, maximum size of the essential assets that the system downloads before it launches your app in bytes.

