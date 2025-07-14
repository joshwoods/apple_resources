

- Foundation
-  NSMetadataQueryNetworkScope 

Global Variable

# NSMetadataQueryNetworkScope

Search all user-mounted remote volumes.

macOS 10.4+

``` source
let NSMetadataQueryNetworkScope: String
```

## See Also

### Constants

let NSMetadataQueryUserHomeScope: String

Search the user’s home directory.

let NSMetadataQueryLocalComputerScope: String

Search all local mounted volumes, including the user home directory. The user’s home directory is searched even if it is a remote volume.

let NSMetadataQueryUbiquitousDocumentsScope: String

Search all files in the `Documents` directories of the app’s iCloud container directories.

let NSMetadataQueryUbiquitousDataScope: String

Search all files not in the `Documents` directories of the app’s iCloud container directories.

let NSMetadataQueryAccessibleUbiquitousExternalDocumentsScope: String

Search for documents outside the app’s container. This search can locate iCloud documents that the user previously opened using a document picker view controller. This lets your app access the documents again without requiring direct user interaction. The result’s NSMetadataItemURLKey attributes return security-scoped NSURLs. For more information on working with security-scoped URLs, see Security-Scoped URLs in NSURL.

let NSMetadataQueryIndexedLocalComputerScope: String

Search all indexed local mounted volumes including the current user’s home directory (even if the home directory is remote).

let NSMetadataQueryIndexedNetworkScope: String

Search all indexed user-mounted remote volumes.

