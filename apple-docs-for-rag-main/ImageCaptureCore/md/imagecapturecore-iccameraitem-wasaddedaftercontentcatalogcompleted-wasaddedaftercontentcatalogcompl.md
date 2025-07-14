

- ImageCaptureCore
- ICCameraItem
-  wasAddedAfterContentCatalogCompleted 

Instance Property

# wasAddedAfterContentCatalogCompleted

A Boolean value indicating whether the item was captured on the camera after the camera’s content had been fully enumerated.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var wasAddedAfterContentCatalogCompleted: Bool { get }
```

## Discussion

This value does not apply to files added as a result of adding a new store to the camera.

## See Also

### Determining an Item’s Change Dates

var creationDate: Date?

The item’s creation date, usually the same as its `EXIF` creation date.

var modificationDate: Date?

The item’s modification date, usually the same as its `EXIF` modification date.

