

- ImageCaptureCore
- ICCameraItem
-  creationDate 

Instance Property

# creationDate

The item’s creation date, usually the same as its `EXIF` creation date.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var creationDate: Date? { get }
```

## See Also

### Determining an Item’s Change Dates

var modificationDate: Date?

The item’s modification date, usually the same as its `EXIF` modification date.

var wasAddedAfterContentCatalogCompleted: Bool

A Boolean value indicating whether the item was captured on the camera after the camera’s content had been fully enumerated.

