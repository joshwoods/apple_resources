

- Foundation
- NSFileVersion
-  isConflict 

Instance Property

# isConflict

A Boolean value indicating whether the contents of the version are in conflict with the contents of another version.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isConflict: Bool { get }
```

## Discussion

When two or more versions of a file are written at the same time, perhaps because the file is saved in the cloud and one or more of the writers were offline when they were writing, the system attempts to resolve the conflict automatically. It does this by picking one of the file versions to be the current file and setting this property to true for the other file versions that are in conflict.

## See Also

### Handling Version Conflicts

var isResolved: Bool

A Boolean value that indicates the version object is not in conflict (true) or is in conflict (false).

class func unresolvedConflictVersionsOfItem(at: URL) -> [NSFileVersion]?

Returns an array of version objects that are currently in conflict for the specified URL.

