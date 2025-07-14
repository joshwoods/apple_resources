

- Bundle Resources
- Information Property List
-  NSRemovableVolumesUsageDescription 

Property List Key

# NSRemovableVolumesUsageDescription

A message that tells the user why the app needs access to files on a removable volume.

macOS 10.15+

## Details 

Name  
Privacy - Removable Volumes Usage Description

Type  

string

## Discussion

The user implicitly grants your app access to a file on a removable volume—like a USB thumb drive—when selecting the file in an Open or Save panel, dragging it onto your app, or opening it in Finder. Your app can access that file right away and any time in the future. In addition, if your app creates a new file on a removable volume, the app can access that file without user consent.

The first time your app tries to access a file on a removable volume without implied user consent, the system prompts the user for permission to access removable volumes. Add the NSRemovableVolumesUsageDescription key to your app’s Information Property List file to provide a string for the prompt that explains why your app needs access. The usage description is optional, but highly recommended.

After the user chooses whether to grant access, the system remembers the user’s choice. To reset permissions, use the `tccutil` command line utility with your app’s bundle ID:

```
$ tccutil reset SystemPolicyRemovableVolumes 
```

## See Also

### Files and folders

NSDesktopFolderUsageDescription

A message that tells the user why the app needs access to the user’s Desktop folder.

**Name:** Privacy - Desktop Folder Usage Description

NSDocumentsFolderUsageDescription

A message that tells the user why the app needs access to the user’s Documents folder.

**Name:** Privacy - Documents Folder Usage Description

NSDownloadsFolderUsageDescription

A message that tells the user why the app needs access to the user’s Downloads folder.

**Name:** Privacy - Downloads Folder Usage Description

NSNetworkVolumesUsageDescription

A message that tells the user why the app needs access to files on a network volume.

**Name:** Privacy - Network Volumes Usage Description

NSFileProviderDomainUsageDescription

A message that tells the user why the app needs access to files managed by a file provider.

**Name:** Privacy - Access to a File Provider Domain Usage Description

