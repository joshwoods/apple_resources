

- WebKit
-  WKSnapshotConfiguration 

Class

# WKSnapshotConfiguration

The configuration data to use when generating an image from a web view’s contents.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
class WKSnapshotConfiguration
```

## Overview

Create a WKSnapshotConfiguration object when you want to generate an image based on your web view’s content. Use this object to specify the portion of the web view to capture and the capture behavior. To generate the snapshot, pass the configuration object to the takeSnapshot(with:completionHandler:) method of WKWebView, which returns a platform-native image for you to use.

## Topics

### Specifying the snapshot dimensions

var rect: CGRect

The portion of your web view to capture, specified as a rectangle in the view’s coordinate system.

var snapshotWidth: NSNumber?

The width of the captured image, in points.

### Configuring the capture behavior

var afterScreenUpdates: Bool

A Boolean value that indicates whether to take the snapshot after incorporating any pending screen updates.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Snapshots

class WKPDFConfiguration

The configuration data to use when generating a PDF representation of a web view’s contents.

