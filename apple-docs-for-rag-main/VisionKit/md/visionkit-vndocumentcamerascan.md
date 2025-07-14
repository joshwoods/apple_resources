

- VisionKit
-  VNDocumentCameraScan 

Class

# VNDocumentCameraScan

A single document scanned in the document camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class VNDocumentCameraScan
```

## Overview

When the document camera scans a document, it returns the resulting information in this format, through the delegate method documentCameraViewController(_:didFinishWith:).

## Topics

### Reading the scanned document

var title: String

The title of the scanned document.

var pageCount: Int

The number of pages in the scanned document.

func imageOfPage(at: Int) -> UIImage

Requests the image of a page at a specified index.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Document scanning through the camera

Structuring Recognized Text on a Document

Detect, recognize, and structure text on a business card or receipt using Vision and VisionKit.

class VNDocumentCameraViewController

An object that presents UI for a camera pass-through that helps people scan physical documents.

protocol VNDocumentCameraViewControllerDelegate

A delegate protocol through which the document camera returns its scanned results.

