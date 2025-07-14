

- AppKit
- NSOpenPanel
-  canDownloadUbiquitousContents 

Instance Property

# canDownloadUbiquitousContents

A Boolean value that indicates how the panel responds to iCloud documents that aren’t fully downloaded locally.

macOS 10.10+

``` source
@MainActor
var canDownloadUbiquitousContents: Bool { get set }
```

## Discussion

When the value of this property is true, the panel disallows opening non-local iCloud files. If the user selects a non-local file, the panel attempts to download that file. When the value of this property is false, the user may select and open non-local files. Your app is responsible for downloading the files and reporting progress or any issues.

The default value of this property is true, except for applications linked against the OS X v10.9 SDK or earlier that have adopted iCloud by specifying a ubiquitous container identifier entitlement.

For a better user experience, set this property to false and download the file’s contents with an NSFileCoordinator object. Show the dlownload progress using a Progress or NSMetadataQuery object.

## See Also

### Supporting iCloud Documents

var canResolveUbiquitousConflicts: Bool

A Boolean value that indicates how the panel responds to iCloud documents that have conflicting versions.

