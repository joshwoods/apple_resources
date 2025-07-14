

- VisionKit
-  VNDocumentCameraViewController 

Class

# VNDocumentCameraViewController

An object that presents UI for a camera pass-through that helps people scan physical documents.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class VNDocumentCameraViewController
```

## Overview

This class enables a person to scan a physical document, page by page, by tapping a camera interface in the controller’s view. The results of a scan include images, by page number. With the collection of scanned images, your app can create a digital version of the physical document and export the scanned images to PDF.

## Present a document scanning view controller in Swift

The following Swift code presents the document scanning object and adds it to your view controller hierarchy:

```
let documentCameraViewController = VNDocumentCameraViewController()
documentCameraViewController.delegate = self
present(documentCameraViewController, animated: true)
```

## Present a document scanning view controller in Objective-C

The following Objective-C code presents the document scanning object and adds it to your view controller hierarchy:

```
```

## Topics

### Supporting the document camera

var delegate: (any VNDocumentCameraViewControllerDelegate)?

The delegate to be notified when the user saves or cancels the document scanner.

class var isSupported: Bool

A Boolean variable that indicates whether or not the current device supports document scanning.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Document scanning through the camera

Structuring Recognized Text on a Document

Detect, recognize, and structure text on a business card or receipt using Vision and VisionKit.

protocol VNDocumentCameraViewControllerDelegate

A delegate protocol through which the document camera returns its scanned results.

class VNDocumentCameraScan

A single document scanned in the document camera.

