

- Foundation
- NSItemProvider
-  loadPreviewImage(options:completionHandler:) 

Instance Method

# loadPreviewImage(options:completionHandler:)

Loads the preview image for the item that the item provider represents.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func loadPreviewImage(
    options: [AnyHashable : Any]! = [:],
    completionHandler: NSItemProvider.CompletionHandler!
)
```

``` source
func loadPreviewImage(options: [AnyHashable : Any]! = [:]) async throws -> any NSSecureCoding
```

## Parameters 

`options`  

A dictionary of keys and values that provide information about the item, such as the size of an image. For a list of possible keys, see Options Dictionary Key.

`completionHandler`  

A completion handler block to execute with the results. The first parameter of this block must be a parameter of type NSData, NSURL, UIImage (in iOS), or NSImage (in macOS) for receiving the image data. For more information about implementing the block, see NSItemProvider.CompletionHandler.

## Discussion

To handle image preview yourself, provide a completion handler block that returns an NSData or NSURL object, or an instance of a platform-specific image class (UIImage or NSImage).

This method supports implicit type coercion for the item parameter of the completion block.

## See Also

### Loading a preview image

var previewImageHandler: NSItemProvider.LoadHandler?

The custom preview image handler block for the item provider.

