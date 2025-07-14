

- Foundation
- NSString
-  abbreviatingWithTildeInPath 

Instance Property

# abbreviatingWithTildeInPath

A new string that replaces the current home directory portion of the current path with a tilde (`~`) character.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var abbreviatingWithTildeInPath: String { get }
```

## Discussion

A new string based on the current string object. If the new string specifies a file in the current home directory, the home directory portion of the path is replaced with a tilde (`~`) character. If the string does not specify a file in the current home directory, this method returns a new string object whose path is unchanged from the path in the current string.

Note that this method only works with file paths. It does not work for string representations of URLs.

For sandboxed apps in macOS, the current home directory is not the same as the user’s home directory. For a sandboxed app, the home directory is the app’s home directory. So if you specified a path of `/Users/`*\*`/file.txt` for a sandboxed app, the returned path would be unchanged from the original. However, if you specified the same path for an app not in a sandbox, this method would replace the `/Users/`*\* portion of the path with a tilde.

## See Also

### Working with Paths

class func path(withComponents: [String]) -> String

Returns a string built from the strings in a given array by concatenating them with a path separator between each pair.

var pathComponents: [String]

The file-system path components of the receiver.

func completePath(into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?, caseSensitive: Bool, matchesInto: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?, filterTypes: [String]?) -> Int

Interprets the receiver as a path in the file system and attempts to perform filename completion, returning a numeric value that indicates whether a match was possible, and by reference the longest path that matches the receiver.

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

