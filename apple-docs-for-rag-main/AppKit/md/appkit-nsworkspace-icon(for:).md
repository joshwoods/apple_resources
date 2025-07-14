

- AppKit
- NSWorkspace
-  icon(for:) 

Instance Method

# icon(for:)

Returns an image containing the icon for the specified content type.

macOS 11.0+

``` source
func icon(for contentType: UTType) -> NSImage
```

## Parameters 

`contentType`  

An object representing a uniform type of content.

## Return Value

The icon associated with the content type.

## Discussion

This method returns a default icon if the operation fails.

## See Also

### Managing Icons

func icon(forFile: String) -> NSImage

Returns an image containing the icon for the specified file.

func icon(forFiles: [String]) -> NSImage?

Returns an image containing the icon for the specified files.

func setIcon(NSImage?, forFile: String, options: NSWorkspace.IconCreationOptions) -> Bool

Sets the icon for the file or directory at the specified path.

struct IconCreationOptions

Constants that describe options for creating icons.

