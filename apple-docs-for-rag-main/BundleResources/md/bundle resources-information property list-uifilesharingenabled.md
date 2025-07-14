

- Bundle Resources
- Information Property List
-  UIFileSharingEnabled 

Property List Key

# UIFileSharingEnabled

A Boolean value indicating whether the app shares files.

iOS 3.2+iPadOS 3.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

## Details 

Name  
Application supports iTunes file sharing

Type  

boolean

## Discussion

If you set this key to `YES`, your app can share files with the user. Place the files in a `Documents` folder located in the app’s home directiory. The default value is `NO`.

## See Also

### Related Documentation

LSSupportsOpeningDocumentsInPlace

A Boolean value indicating whether the app may open the original document from a file provider, rather than a copy of the document.

**Name:** Supports opening documents in place

func NSHomeDirectory() -> String

Returns the path to either the user’s or application’s home directory, depending on the platform.

### Storage

APFiles

Describes the files or directories the app installs on the system.

**Name:** Installation files

APInstallerURL

The base path to the files or folders that the app installs.

**Name:** Installation directory base file URL

NSSupportsPurgeableLocalStorage

A Boolean value indicating whether the app continues working if the system purges the local storage.

LSFileQuarantineEnabled

A Boolean value indicating whether the files this app creates are quarantined by default.

**Name:** File quarantine enabled

CSResourcesFileMapped

A Boolean value indicating whether the app’s resources files should be mapped into memory.

**Name:** Resources should be file-mapped

NSDownloadsUbiquitousContents

A Boolean value that indicates whether the system should download documents before handing them over to the app.

