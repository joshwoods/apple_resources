

- Foundation
- NSString
-  appendingPathExtension(\_:) 

Instance Method

# appendingPathExtension(\_:)

Returns a new string made by appending to the receiver an extension separator followed by a given extension.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func appendingPathExtension(_ str: String) -> String?
```

## Parameters 

`str`  

The extension to append to the receiver.

## Return Value

A new string made by appending to the receiver an extension separator followed by `ext`.

## Discussion

The following table illustrates the effect of this method on a variety of different paths, assuming that `ext` is supplied as `@"tiff"`:

| Receiver’s String Value | Resulting String          |
|-------------------------|---------------------------|
| “`/tmp/scratch.old`”    | “`/tmp/scratch.old.tiff`” |
| “`/tmp/scratch.`”       | “`/tmp/scratch..tiff`”    |
| “`/tmp/`”               | “`/tmp.tiff`”             |
| “`scratch`”             | “`scratch.tiff`”          |

Note that adding an extension to `@"/tmp/"` causes the result to be `@"/tmp.tiff"` instead of `@"/tmp/.tiff"`. This difference is because a file named `@".tiff"` is not considered to have an extension, so the string is appended to the last nonempty path component.

Note that this method only works with file paths (not, for example, string representations of URLs).

### Special Considerations

Prior to OS X v10.9 this method did not allow you to append file extensions to filenames starting with the tilde character (`~`).

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

var abbreviatingWithTildeInPath: String

A new string that replaces the current home directory portion of the current path with a tilde (`~`) character.

func appendingPathComponent(String) -> String

Returns a new string made by appending to the receiver a given string.

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

