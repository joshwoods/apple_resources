

- AppKit
- NSWorkspace
-  setIcon(\_:forFile:options:) 

Instance Method

# setIcon(\_:forFile:options:)

Sets the icon for the file or directory at the specified path.

macOS

``` source
func setIcon(
    _ image: NSImage?,
    forFile fullPath: String,
    options: NSWorkspace.IconCreationOptions = []
) -> Bool
```

## Parameters 

`image`  

The image to use as the icon for the file or directory.

`fullPath`  

The full path of the file or directory.

`options`  

The icon representations to generate from the image. You specify this value by combining the appropriate NSWorkspace.IconCreationOptions constants, using the C bitwise `OR` operator. Specify `0` if you want to generate icons in all available icon representation formats.

## Return Value

true if the icon was set; otherwise, false.

## Discussion

The `image` can be an arbitrary image, with or without transparency. The method automatically scales this image (as needed) to generate the icon representations. The file or folder must exist and be writable by the user.

This method uses the image to set an icon with a size of 512 pixels by 512 pixels. If you specify the exclude10_4ElementsIconCreationOption option (not recommended), this method creates an icon that is compatible with the Finder from macOS 10.2 or earlier.

You can safely call this method from any of your app’s threads, but you must call it from only one thread at a time.

## See Also

### Managing Icons

func icon(forFile: String) -> NSImage

Returns an image containing the icon for the specified file.

func icon(forFiles: [String]) -> NSImage?

Returns an image containing the icon for the specified files.

func icon(for: UTType) -> NSImage

Returns an image containing the icon for the specified content type.

struct IconCreationOptions

Constants that describe options for creating icons.

