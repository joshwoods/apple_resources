

- Foundation
- Bundle
-  pathForImageResource(\_:) 

Instance Method

# pathForImageResource(\_:)

Returns the location of the specified image resource file.

macOS 10.0+

``` source
func pathForImageResource(_ name: NSImage.Name) -> String?
```

## Parameters 

`name`  

The name of the image resource file, without any pathname information. Including a filename extension is optional.

## Return Value

The absolute pathname of the resource file or `nil` if the file is not found.

## Discussion

Image resources are those files in the bundle that are recognized by the `NSImage` class, including those that can be converted using the Image IO framework.

## See Also

### Related Documentation

func path(forResource: String?, ofType: String?) -> String?

Returns the full pathname for the resource identified by the specified name and file extension.

### Finding Image Resources

func urlForImageResource(NSImage.Name) -> URL?

Returns the location of the specified image resource as an NSURL.

func image(forResource: NSImage.Name) -> NSImage?

Returns an `NSImage` instance associated with the specified name, which can be backed by multiple files representing different resolution versions of the image.

