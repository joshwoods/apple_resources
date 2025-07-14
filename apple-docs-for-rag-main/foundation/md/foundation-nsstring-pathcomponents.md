

- Foundation
- NSString
-  pathComponents 

Instance Property

# pathComponents

The file-system path components of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var pathComponents: [String] { get }
```

## Discussion

The strings in the array appear in the order they did in the receiver. If the string begins or ends with the path separator, then the first or last component, respectively, will contain the separator. Empty components (caused by consecutive path separators) are deleted. For example, this code excerpt:

```
NSString *path = @"tmp/scratch";
NSArray *pathComponents = [path pathComponents];
```

produces an array with these contents:

| Index | Path Component |
|-------|----------------|
| 0     | “`tmp`”        |
| 1     | “`scratch`”    |

If the receiver begins with a slash—for example, “`/tmp/scratch`”—the array has these contents:

| Index | Path Component |
|-------|----------------|
| 0     | “`/`”          |
| 1     | “`tmp`”        |
| 2     | “`scratch`”    |

If the receiver has no separators—for example, “`scratch`”—the array contains the string itself, in this case “`scratch`”.

Note that this method only works with file paths—not, for example, string representations of URLs.

## See Also

### Related Documentation

func components(separatedBy: String) -> [String]

Returns an array containing substrings from the receiver that have been divided by a given separator.

### Working with Paths

class func path(withComponents: [String]) -> String

Returns a string built from the strings in a given array by concatenating them with a path separator between each pair.

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

