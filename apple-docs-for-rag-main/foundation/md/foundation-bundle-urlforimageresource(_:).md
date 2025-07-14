

- Foundation
- Bundle
-  urlForImageResource(\_:) 

Instance Method

# urlForImageResource(\_:)

Returns the location of the specified image resource as an NSURL.

macOS 10.6+

``` source
func urlForImageResource(_ name: NSImage.Name) -> URL?
```

## Parameters 

`name`  

The name of the image resource file. Including a filename extension is optional.

## Return Value

An `NSURL` for the resource file or `nil` if the file was not found.

## See Also

### Finding Image Resources

func pathForImageResource(NSImage.Name) -> String?

Returns the location of the specified image resource file.

func image(forResource: NSImage.Name) -> NSImage?

Returns an `NSImage` instance associated with the specified name, which can be backed by multiple files representing different resolution versions of the image.

