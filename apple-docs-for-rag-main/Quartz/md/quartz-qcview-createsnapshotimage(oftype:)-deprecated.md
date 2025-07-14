

- Quartz
- QCView
-  createSnapshotImage(ofType:) Deprecated

Instance Method

# createSnapshotImage(ofType:)

Returns the current image in the view as an image object of the provided image type.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func createSnapshotImage(ofType type: String!) -> Any!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`type`  

A string that specifies any of the following image types: NSBitmapImageRep, NSImage, CIImage, `CGImage`, `CVOpenGLBuffer`, `CVPixelBuffer`.

## Return Value

The snapshot image in the provided image type. You are responsible for releasing this object when you no longer need it.

## See Also

### Taking Snapshot Images

func snapshotImage() -> NSImage!

Returns an `NSImage` object of the current image in the view.

Deprecated

