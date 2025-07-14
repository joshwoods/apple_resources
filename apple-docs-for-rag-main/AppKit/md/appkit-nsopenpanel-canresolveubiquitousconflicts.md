

- AppKit
- NSOpenPanel
-  canResolveUbiquitousConflicts 

Instance Property

# canResolveUbiquitousConflicts

A Boolean value that indicates how the panel responds to iCloud documents that have conflicting versions.

macOS 10.10+

``` source
@MainActor
var canResolveUbiquitousConflicts: Bool { get set }
```

## Discussion

When the value of this property is true, and the user attempts to open one or more documents with conflicts, the panel displays the conflict resolution UI. The user must resolve any conflicts before opening the documents. When the value of this property is false, the your application is responsible for handling any conflicts.

The default value of this property is true, except for applications linked against the OS X v10.9 SDK or earlier that have adopted iCloud by specifying a ubiquitous container identifier entitlement.

For a better user experience, set this property to false and check the ubiquitousItemHasUnresolvedConflictsKey key of each item. When a conflict exists, retrieve a NSFileVersion object for each version and present your own UI to resolve that conflict.

## See Also

### Supporting iCloud Documents

var canDownloadUbiquitousContents: Bool

A Boolean value that indicates how the panel responds to iCloud documents that aren’t fully downloaded locally.

