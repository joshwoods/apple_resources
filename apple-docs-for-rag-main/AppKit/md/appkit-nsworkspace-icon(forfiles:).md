

- AppKit
- NSWorkspace
-  icon(forFiles:) 

Instance Method

# icon(forFiles:)

Returns an image containing the icon for the specified files.

macOS

``` source
func icon(forFiles fullPaths: [String]) -> NSImage?
```

## Parameters 

`fullPaths`  

An array of `NSString` objects, each of which contains the full path to a file.

## Return Value

The icon associated with the group of files.

## Discussion

If `fullPaths` specifies one file, that file’s icon is returned. If `fullPaths` specifies more than one file, an icon representing the multiple selection is returned.

You can safely call this method from any thread of your app.

## See Also

### Related Documentation

func icon(forFileType: String) -> NSImage

Returns an image containing the icon for files of the specified type.

Deprecated

### Managing Icons

func icon(forFile: String) -> NSImage

Returns an image containing the icon for the specified file.

func icon(for: UTType) -> NSImage

Returns an image containing the icon for the specified content type.

func setIcon(NSImage?, forFile: String, options: NSWorkspace.IconCreationOptions) -> Bool

Sets the icon for the file or directory at the specified path.

struct IconCreationOptions

Constants that describe options for creating icons.

