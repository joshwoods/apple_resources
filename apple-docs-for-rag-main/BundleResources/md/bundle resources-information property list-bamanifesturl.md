

- Bundle Resources
- Information Property List
-  BAManifestURL 

Property List Key

# BAManifestURL

The location URL of the app’s manifest file that contains the names and sizes of assets.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

## Details 

Type  

string

## Discussion

The manifest file contains information that your extension needs to schedule asset downloads, such as the names, URLs, and sizes of the assets. The format and content of the manifest file is your responsibility. The system uses this key to download the manifest file and pass it to your extension. This key is required to use Background Assets.

## See Also

### Background downloads

BAInitialDownloadRestrictions

The restrictions that apply to the set of assets that download immediately after app installation.

BAMaxInstallSize

The combined, maximum size, in bytes, of the non-essential assets that download immediately after app installation.

BAEssentialMaxInstallSize

The combined, maximum size of the essential assets that the system downloads before it launches your app in bytes.

