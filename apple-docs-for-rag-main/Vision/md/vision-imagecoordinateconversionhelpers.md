

- Vision
-  ImageCoordinateConversionHelpers 

Structure

# ImageCoordinateConversionHelpers

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct ImageCoordinateConversionHelpers
```

## Topics

### Type Methods

static func imagePointForNormalizedPoint(normalizedPoint: CGPoint, imageSize: CGSize) -> CGPoint

static func imageRectForNormalizedRect(normalizedRect: CGRect, imageSize: CGSize) -> CGRect

static func verticallyFlippedImagePoint(imagePoint: CGPoint, imageHeight: UInt32) -> CGPoint

static func verticallyFlippedImageRect(imageRect: CGRect, imageHeight: UInt32) -> CGRect

static func verticallyFlippedNormalizedPoint(normalizedPoint: CGPoint) -> CGPoint

static func verticallyFlippedNormalizedRect(normalizedRect: CGRect, imageHeight: UInt32) -> CGRect

