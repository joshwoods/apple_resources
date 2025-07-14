

- Foundation
- NSItemProvider
-  previewImageHandler 

Instance Property

# previewImageHandler

The custom preview image handler block for the item provider.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var previewImageHandler: NSItemProvider.LoadHandler? { get set }
```

## Discussion

In your image handler block, return an NSURL object that specifies a file, or return an NSData object.

## See Also

### Loading a preview image

func loadPreviewImage(options: [AnyHashable : Any]!, completionHandler: NSItemProvider.CompletionHandler!)

Loads the preview image for the item that the item provider represents.

