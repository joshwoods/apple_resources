

- ImageCaptureCore
-  ICCameraItem 

Class

# ICCameraItem

An abstract class that represents a camera item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
class ICCameraItem
```

## Overview

The ImageCaptureCore framework defines two concrete subclasses of camera items: ICCameraFolder and ICCameraFile.

## Topics

### Inspecting an Item’s Name and Type

var uti: String?

The item’s uniform type identifier (UTI) string.

var name: String?

The item’s name.

var ptpObjectHandle: UInt32

The item’s `PTP` object handle value, if the camera uses the `PTP` protocol.

var isRaw: Bool

A Boolean value indicating whether the item is a raw image file.

### Determining an Item’s Change Dates

var creationDate: Date?

The item’s creation date, usually the same as its `EXIF` creation date.

var modificationDate: Date?

The item’s modification date, usually the same as its `EXIF` modification date.

var wasAddedAfterContentCatalogCompleted: Bool

A Boolean value indicating whether the item was captured on the camera after the camera’s content had been fully enumerated.

### Locating an Item

var device: ICCameraDevice?

The item’s parent device.

var fileSystemPath: String?

The item’s file system path on a camera using the mass storage transport type.

var parentFolder: ICCameraFolder?

This item’s parent folder.

var isInTemporaryStore: Bool

A Boolean value that indicates whether this item is in a temporary store.

### Requesting Metadata

func requestMetadata()

Requests metadata for the item.

var metadata: [AnyHashable : Any]?

The item’s metadata.

var metadataIfAvailable: [String : Any]?

The item’s metadata if it is readily available.

func flushMetadataCache()

Deletes the item’s cached metadata.

struct ICCameraItemMetadataOption

An option for the item’s metadata.

### Requesting Thumbnails

func requestThumbnail()

Requests a thumbnail for the item.

var thumbnail: CGImage?

The item’s thumbnail.

var thumbnailIfAvailable: CGImage?

The item’s thumbnail if it is readily available.

var largeThumbnailIfAvailable: CGImage?

A large thumbnail for the item if one is readily available.

func flushThumbnailCache()

Deletes the item’s cached thumbnail.

struct ICCameraItemThumbnailOption

An option for the item’s thumbnail.

### Accessing a Protected Item

var isLocked: Bool

A Boolean value that indicates whether the storage card in the camera is locked.

### Storing Information

var userData: NSMutableDictionary?

A mutable dictionary to store arbitrary key-value pairs associated with a camera item.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ICCameraFile
- ICCameraFolder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Cameras

class ICCameraDevice

An object that represents a camera.

protocol ICCameraDeviceDelegate

Methods for detecting cameras, getting metadata and thumbnails, handling access and capability changes, and performing other actions on connected cameras.

class ICCameraFile

An object that represents a file on a camera.

class ICCameraFolder

An object that represents a folder on a camera.

