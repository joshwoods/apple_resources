

- Bundle Resources
- Information Property List
-  APFiles 

Property List Key

# APFiles

Describes the files or directories the app installs on the system.

macOS 10.0+

## Details 

Name  
Installation files

Type  

object

## Topics

### Property List Keys

APDisplayedAsContainer

A Boolean value indicating whether the file or a folder icon is displayed in the Info window.

**Name:** Display with folder icon

APFileDescriptionKey

A short description of the file or folder that appears in the Info window.

**Name:** Install file description text

APFileDestinationPath

The path to use when installing the file or folder, relative to the app bundle.

**Name:** File destination path

APFileName

The name of the file or folder to install.

**Name:** Install file name

APFileSourcePath

The path to the file or folder in the app package, relative to the installer path.

**Name:** Install file source path

APInstallAction

The action to take on the file or folder.

**Name:** File install action

## See Also

### Storage

APInstallerURL

The base path to the files or folders that the app installs.

**Name:** Installation directory base file URL

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

