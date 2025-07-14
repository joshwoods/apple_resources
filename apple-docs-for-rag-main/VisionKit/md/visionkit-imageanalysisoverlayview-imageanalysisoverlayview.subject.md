

- VisionKit
- ImageAnalysisOverlayView
-  ImageAnalysisOverlayView.Subject 

Structure

# ImageAnalysisOverlayView.Subject

An area of interest in an image that the framework identifies as a primary focal point.

macOS 13.0+

``` source
struct Subject
```

## Overview

A *subject* is a foreground object in an image. A single image can have multiple subjects. For example, in an image of three different coffee mugs, the framework may classify all three mugs as separate subjects. In cases where the framework can’t separate overlapping objects in a photo as individual subjects, a subject may consist of two or more objects.

VisionKit enables your app to extract, or *lift*, the image subjects individually, or together, with the background removed. For more information, see image.

An ImageAnalysisOverlayView object contains an array of subjects (subjects) that activates when preferredInteractionTypes contains a subject-related option, such as automatic, or imageSubject.

Your app can also present a button that gives more information on an image’s subjects by enabling the visualLookUp interaction type.

## Topics

### Acquiring the subject image

var image: NSImage

An image of the subjects with the background removed.

### Locating and sizing the subject

var bounds: CGRect

A rectangle that identifies the extremities of a subject within an image.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Accessing image subjects

var subjects: Set&lt;ImageAnalysisOverlayView.Subject>

The set of all subjects the framework identifies in an image.

func image(for: Set&lt;ImageAnalysisOverlayView.Subject>) async throws -> NSImage

Provides an image asynchronously that contains the given subjects with the background removed.

func subject(at: CGPoint) async -> ImageAnalysisOverlayView.Subject?

Returns the subject at the given point within the overlay view’s image, if one exists.

