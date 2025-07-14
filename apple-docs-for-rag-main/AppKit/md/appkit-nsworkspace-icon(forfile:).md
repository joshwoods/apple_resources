

- AppKit
- NSWorkspace
-  icon(forFile:) 

Instance Method

# icon(forFile:)

Returns an image containing the icon for the specified file.

macOS

``` source
func icon(forFile fullPath: String) -> NSImage
```

## Parameters 

`fullPath`  

The full path to the file.

## Return Value

The icon associated with the file.

## Discussion

The returned image has an initial size of 32 pixels by 32 pixels.

You can safely call this method from any thread of your app.

## See Also

### Related Documentation

func icon(forFileType: String) -> NSImage

Returns an image containing the icon for files of the specified type.

Deprecated

func getInfoForFile(String, application: AutoreleasingUnsafeMutablePointer&lt;NSString?>?, type: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Retrieves information about the specified file.

Deprecated

### Managing Icons

func icon(forFiles: [String]) -> NSImage?

Returns an image containing the icon for the specified files.

func icon(for: UTType) -> NSImage

Returns an image containing the icon for the specified content type.

func setIcon(NSImage?, forFile: String, options: NSWorkspace.IconCreationOptions) -> Bool

Sets the icon for the file or directory at the specified path.

struct IconCreationOptions

Constants that describe options for creating icons.

