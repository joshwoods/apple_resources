

- WebKit
-  WKPDFConfiguration 

Class

# WKPDFConfiguration

The configuration data to use when generating a PDF representation of a web view’s contents.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS 1.0+

``` source
@MainActor
class WKPDFConfiguration
```

## Overview

Create a WKPDFConfiguration object when you want to generate a PDF version of your web view’s content. Use this object to specify the portion of the web view to capture. To generate the PDF content, pass the configuration object to the createPDF(configuration:completionHandler:) method of WKWebView, which returns the PDF data for you to use.

## Topics

### Specifying the snapshot dimensions

var rect: CGRect?

The portion of your web view to capture, specified as a rectangle in the view’s coordinate system.

### Specifying snapshot properties

var allowTransparentBackground: Bool

A Boolean value that indicates whether the PDF may have a transparent background.

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

class WKSnapshotConfiguration

The configuration data to use when generating an image from a web view’s contents.

