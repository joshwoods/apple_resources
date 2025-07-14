

- SceneKit
-  SCNSceneExportDelegate 

Protocol

# SCNSceneExportDelegate

Methods you can implement to participate in the process of exporting a scene to a file.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.9+tvOS 10.0+visionOS 1.0+

``` source
protocol SCNSceneExportDelegate : NSObjectProtocol
```

## Overview

When you call a SCNScene object’s write(to:options:delegate:progressHandler:) method to export the scene’s content to a file, you can optionally specify a delegate object to receive these messages.

## Topics

### Writing Image Attachments

func write(UIImage, withSceneDocumentURL: URL, originalImageURL: URL?) -> URL?

Tells the delegate to export an image attached to a scene.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Exporting a Scene File

func write(to: URL, options: [String : Any]?, delegate: (any SCNSceneExportDelegate)?, progressHandler: SCNSceneExportProgressHandler?) -> Bool

Exports the scene and its contents to a file at the specified URL.

