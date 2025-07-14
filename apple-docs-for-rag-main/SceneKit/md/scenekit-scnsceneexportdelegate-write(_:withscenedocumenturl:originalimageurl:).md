

- SceneKit
- SCNSceneExportDelegate
-  write(\_:withSceneDocumentURL:originalImageURL:) 

Instance Method

# write(\_:withSceneDocumentURL:originalImageURL:)

Tells the delegate to export an image attached to a scene.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.9+tvOS 10.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
optional func write(
    _ image: UIImage,
    withSceneDocumentURL documentURL: URL,
    originalImageURL: URL?
) -> URL?
```

**macOS**

``` source
optional func write(
    _ image: NSImage,
    withSceneDocumentURL documentURL: URL,
    originalImageURL: URL?
) -> URL?
```

## Parameters 

`image`  

An image attached to the scene being exported.

`documentURL`  

The URL the scene is being exported to.

`originalImageURL`  

The URL the image was originally loaded from, or `nil` if the image was not previously loaded from a URL.

## Return Value

The URL your app exported the image to, or `nil` if your app did not write the image to a URL.

## Discussion

If you implement this method, Scene Kit calls it for each image (for example, a texture) attached to the scene. Your app can then save the image data in a location and format of your choice, returning a URL for the exported image file.

If you do not provide a delegate when exporting a scene, or if your delegate returns `nil` from this method, Scene Kit exports the image in a default format to a default location.

