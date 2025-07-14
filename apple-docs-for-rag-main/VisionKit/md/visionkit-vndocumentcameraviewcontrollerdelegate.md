

- VisionKit
-  VNDocumentCameraViewControllerDelegate 

Protocol

# VNDocumentCameraViewControllerDelegate

A delegate protocol through which the document camera returns its scanned results.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
protocol VNDocumentCameraViewControllerDelegate : NSObjectProtocol
```

## Overview

Your app is responsible for dismissing the document camera in all delegate callback methods.

## Topics

### Determining scan results

func documentCameraViewController(VNDocumentCameraViewController, didFinishWith: VNDocumentCameraScan)

Tells the delegate that the user successfully saved a scanned document from the document camera.

func documentCameraViewControllerDidCancel(VNDocumentCameraViewController)

Tells the delegate that the user canceled out of the document scanner camera.

func documentCameraViewController(VNDocumentCameraViewController, didFailWithError: any Error)

Tells the delegate that document scanning failed while the camera view controller was active.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Document scanning through the camera

Structuring Recognized Text on a Document

Detect, recognize, and structure text on a business card or receipt using Vision and VisionKit.

class VNDocumentCameraViewController

An object that presents UI for a camera pass-through that helps people scan physical documents.

class VNDocumentCameraScan

A single document scanned in the document camera.

