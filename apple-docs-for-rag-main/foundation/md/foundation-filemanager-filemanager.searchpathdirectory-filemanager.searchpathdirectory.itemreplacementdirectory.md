

- Foundation
- FileManager
- FileManager.SearchPathDirectory
-  FileManager.SearchPathDirectory.itemReplacementDirectory 

Case

# FileManager.SearchPathDirectory.itemReplacementDirectory

The constant used to create a temporary directory.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case itemReplacementDirectory
```

## Discussion

Pass this constant to the FileManager method url(for:in:appropriateFor:create:) in order to create a temporary directory.

## See Also

### Directory Locations

case applicationDirectory

Supported applications (`/Applications`).

case demoApplicationDirectory

Unsupported applications and demonstration versions.

case developerApplicationDirectory

Developer applications (`/Developer/Applications`).

case adminApplicationDirectory

System and network administration applications.

case libraryDirectory

Various user-visible documentation, support, and configuration files (`/Library`).

case developerDirectory

Developer resources (`/Developer`).

case userDirectory

User home directories (`/Users`).

case documentationDirectory

Documentation.

case documentDirectory

Document directory.

case coreServiceDirectory

Core services (`System/Library/CoreServices`).

case autosavedInformationDirectory

The user’s autosaved documents (`Library/Autosave Information`).

case desktopDirectory

The user’s desktop directory.

case cachesDirectory

Discardable cache files (`Library/Caches`).

case applicationSupportDirectory

Application support files (`Library/Application Support`).

case downloadsDirectory

The user’s downloads directory.

