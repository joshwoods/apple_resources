

- Foundation
-  NSMetadataQueryAccessibleUbiquitousExternalDocumentsScope 

Global Variable

# NSMetadataQueryAccessibleUbiquitousExternalDocumentsScope

Search for documents outside the app’s container. This search can locate iCloud documents that the user previously opened using a document picker view controller. This lets your app access the documents again without requiring direct user interaction. The result’s NSMetadataItemURLKey attributes return security-scoped NSURLs. For more information on working with security-scoped URLs, see Security-Scoped URLs in NSURL.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSMetadataQueryAccessibleUbiquitousExternalDocumentsScope: String
```

## See Also

### Constants

let NSMetadataQueryUserHomeScope: String

Search the user’s home directory.

let NSMetadataQueryLocalComputerScope: String

Search all local mounted volumes, including the user home directory. The user’s home directory is searched even if it is a remote volume.

let NSMetadataQueryNetworkScope: String

Search all user-mounted remote volumes.

let NSMetadataQueryUbiquitousDocumentsScope: String

Search all files in the `Documents` directories of the app’s iCloud container directories.

let NSMetadataQueryUbiquitousDataScope: String

Search all files not in the `Documents` directories of the app’s iCloud container directories.

let NSMetadataQueryIndexedLocalComputerScope: String

Search all indexed local mounted volumes including the current user’s home directory (even if the home directory is remote).

let NSMetadataQueryIndexedNetworkScope: String

Search all indexed user-mounted remote volumes.

