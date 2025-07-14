

- Bundle Resources
- Information Property List
-  NSDesktopFolderUsageDescription 

Property List Key

# NSDesktopFolderUsageDescription

A message that tells the user why the app needs access to the user’s Desktop folder.

macOS 10.15+

## Details 

Name  
Privacy - Desktop Folder Usage Description

Type  

string

## Discussion

The user implicitly grants your app access to a file in the Desktop folder when selecting the file in an Open or Save panel, dragging it onto your app, or opening it in Finder. Your app can access that file right away and any time in the future. In addition, if your app creates a new file in the Desktop folder, the app can access that file without user consent.

The first time your app tries to access a file in the user’s Desktop folder without implied user consent, the system prompts the user for permission to access the folder’s contents. Add the NSDesktopFolderUsageDescription key to your app’s Information Property List file to provide a message that explains why your app needs access. The usage description is optional, but highly recommended.

App Sandbox enforces stricter limits on Desktop folder access, so that policy may supersede this one if your app enables sandboxing. See App Sandbox for more information.

After the user chooses whether to grant access, the system remembers the user’s choice. To reset permissions, use the `tccutil` command line utility with your app’s bundle ID:

```
$ tccutil reset SystemPolicyDesktopFolder 
```

## See Also

### Files and folders

NSDocumentsFolderUsageDescription

A message that tells the user why the app needs access to the user’s Documents folder.

**Name:** Privacy - Documents Folder Usage Description

NSDownloadsFolderUsageDescription

A message that tells the user why the app needs access to the user’s Downloads folder.

**Name:** Privacy - Downloads Folder Usage Description

NSNetworkVolumesUsageDescription

A message that tells the user why the app needs access to files on a network volume.

**Name:** Privacy - Network Volumes Usage Description

NSRemovableVolumesUsageDescription

A message that tells the user why the app needs access to files on a removable volume.

**Name:** Privacy - Removable Volumes Usage Description

NSFileProviderDomainUsageDescription

A message that tells the user why the app needs access to files managed by a file provider.

**Name:** Privacy - Access to a File Provider Domain Usage Description

