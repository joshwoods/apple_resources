

- Quartz
- QCRenderer
-  snapshotImage() Deprecated

Instance Method

# snapshotImage()

Returns an `NSImage` object of the current image in the OpenGL context associated with the renderer.

macOS 10.4–10.15Deprecated

``` source
func snapshotImage() -> NSImage!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The snapshot image.

## See Also

### Taking Snapshot Images

func createSnapshotImage(ofType: String!) -> Any!

Returns the current image in the OpenGL context associated with the renderer, as an image object of the provided image type.

Deprecated

