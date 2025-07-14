

- ImageCaptureCore
- ICCameraItem
-  modificationDate 

Instance Property

# modificationDate

The item’s modification date, usually the same as its `EXIF` modification date.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var modificationDate: Date? { get }
```

## See Also

### Determining an Item’s Change Dates

var creationDate: Date?

The item’s creation date, usually the same as its `EXIF` creation date.

var wasAddedAfterContentCatalogCompleted: Bool

A Boolean value indicating whether the item was captured on the camera after the camera’s content had been fully enumerated.

