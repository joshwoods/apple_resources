

- Foundation
- FileManager
-  FileManager.SearchPathDirectory 

Enumeration

# FileManager.SearchPathDirectory

The location of significant directories.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum SearchPathDirectory
```

## Overview

Use these constants with the init(for:in:appropriateFor:create:) initializer and the urls(for:in:) and url(for:in:appropriateFor:create:) methods of FileManager.

## Topics

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

case inputMethodsDirectory

Input Methods `(Library/Input Methods)`.

case moviesDirectory

The user’s Movies directory `(~/Movies`).

case musicDirectory

The user’s Music directory (`~/Music`).

case picturesDirectory

The user’s Pictures directory (`~/Pictures`).

case printerDescriptionDirectory

The system’s PPDs directory (`Library/Printers/PPDs`).

case sharedPublicDirectory

The user’s Public sharing directory (`~/Public`).

case preferencePanesDirectory

The PreferencePanes directory for use with System Preferences (`Library/PreferencePanes`).

case applicationScriptsDirectory

The user scripts folder for the calling application (`~/Library/Application Scripts/`.

case itemReplacementDirectory

The constant used to create a temporary directory.

case allApplicationsDirectory

All directories where applications can be stored.

case allLibrariesDirectory

All directories where resources can be stored.

case trashDirectory

The trash directory.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Types

struct DirectoryEnumerationOptions

Options for enumerating the contents of directories.

struct SearchPathDomainMask

Domain constants specifying base locations to use when you search for significant directories.

struct FileAttributeKey

Keys in dictionaries used to get and set file attributes.

struct FileAttributeType

Values representing a file’s type attribute.

struct FileProtectionType

Protection level values that can be associated with a file attribute key.

struct URLFileProtection

Protection-level values for a URL resource key.

