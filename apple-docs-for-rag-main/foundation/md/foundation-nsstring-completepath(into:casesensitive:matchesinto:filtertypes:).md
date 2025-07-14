

- Foundation
- NSString
-  completePath(into:caseSensitive:matchesInto:filterTypes:) 

Instance Method

# completePath(into:caseSensitive:matchesInto:filterTypes:)

Interprets the receiver as a path in the file system and attempts to perform filename completion, returning a numeric value that indicates whether a match was possible, and by reference the longest path that matches the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func completePath(
    into outputName: AutoreleasingUnsafeMutablePointer?,
    caseSensitive flag: Bool,
    matchesInto outputArray: AutoreleasingUnsafeMutablePointer?,
    filterTypes: [String]?
) -> Int
```

## Parameters 

`outputName`  

Upon return, contains the longest path that matches the receiver.

`flag`  

If true, the method considers case for possible completions.

`outputArray`  

Upon return, contains all matching filenames.

`filterTypes`  

An array of `NSString` objects specifying path extensions to consider for completion. Only paths whose extensions (not including the extension separator) match one of these strings are included in `outputArray`. Pass `nil` if you don’t want to filter the output.

## Return Value

`0` if no matches are found and `1` if exactly one match is found. In the case of multiple matches, returns the actual number of matching paths if `outputArray` is provided, or simply a positive value if `outputArray` is `NULL`.

## Discussion

You can check for the existence of matches without retrieving by passing `NULL` as `outputArray`.

Note that this method only works with file paths (not, for example, string representations of URLs).

## See Also

### Working with Paths

class func path(withComponents: [String]) -> String

Returns a string built from the strings in a given array by concatenating them with a path separator between each pair.

var pathComponents: [String]

The file-system path components of the receiver.

var fileSystemRepresentation: UnsafePointer&lt;CChar>

A file system-specific representation of the receiver.

func getFileSystemRepresentation(UnsafeMutablePointer&lt;CChar>, maxLength: Int) -> Bool

Interprets the receiver as a system-independent path and fills a buffer with a C-string in a format and encoding suitable for use with file-system calls.

var isAbsolutePath: Bool

A Boolean value that indicates whether the receiver represents an absolute path.

var lastPathComponent: String

The last path component of the receiver.

var pathExtension: String

The path extension, if any, of the string as interpreted as a path.

var abbreviatingWithTildeInPath: String

A new string that replaces the current home directory portion of the current path with a tilde (`~`) character.

func appendingPathComponent(String) -> String

Returns a new string made by appending to the receiver a given string.

func appendingPathExtension(String) -> String?

Returns a new string made by appending to the receiver an extension separator followed by a given extension.

var deletingLastPathComponent: String

A new string made by deleting the last path component from the receiver, along with any final path separator.

var deletingPathExtension: String

A new string made by deleting the extension (if any, and only the last) from the receiver.

var expandingTildeInPath: String

A new string made by expanding the initial component of the receiver to its full path value.

var resolvingSymlinksInPath: String

A new string made from the receiver by resolving all symbolic links and standardizing path.

var standardizingPath: String

A new string made by removing extraneous path components from the receiver.

