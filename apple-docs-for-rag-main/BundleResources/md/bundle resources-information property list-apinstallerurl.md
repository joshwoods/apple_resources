

- Bundle Resources
- Information Property List
-  APInstallerURL 

Property List Key

# APInstallerURL

The base path to the files or folders that the app installs.

macOS 10.0+

## Details 

Name  
Installation directory base file URL

Type  

string

## Discussion

Use the format `file://localhost/path/` for the path.

## See Also

### Storage

APFiles

Describes the files or directories the app installs on the system.

**Name:** Installation files

NSSupportsPurgeableLocalStorage

A Boolean value indicating whether the app continues working if the system purges the local storage.

LSFileQuarantineEnabled

A Boolean value indicating whether the files this app creates are quarantined by default.

**Name:** File quarantine enabled

UIFileSharingEnabled

A Boolean value indicating whether the app shares files.

**Name:** Application supports iTunes file sharing

CSResourcesFileMapped

A Boolean value indicating whether the app’s resources files should be mapped into memory.

**Name:** Resources should be file-mapped

NSDownloadsUbiquitousContents

A Boolean value that indicates whether the system should download documents before handing them over to the app.

