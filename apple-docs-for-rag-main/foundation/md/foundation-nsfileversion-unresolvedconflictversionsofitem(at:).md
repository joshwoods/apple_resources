

- Foundation
- NSFileVersion
-  unresolvedConflictVersionsOfItem(at:) 

Type Method

# unresolvedConflictVersionsOfItem(at:)

Returns an array of version objects that are currently in conflict for the specified URL.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func unresolvedConflictVersionsOfItem(at url: URL) -> [NSFileVersion]?
```

## Parameters 

`url`  

The URL of the file that has associated version objects.

## Return Value

An array of `NSFileVersion` objects that represent the versions in conflict or `nil` if the file at URL does not exist.

## See Also

### Handling Version Conflicts

var isConflict: Bool

A Boolean value indicating whether the contents of the version are in conflict with the contents of another version.

var isResolved: Bool

A Boolean value that indicates the version object is not in conflict (true) or is in conflict (false).

