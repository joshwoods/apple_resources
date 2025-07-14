

- Core Image
- CIFilter
-  CIFilterProtocol 

Protocol

# CIFilterProtocol

The properties you use to configure a Core Image filter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIFilterProtocol
```

## Topics

### Instance Properties

var outputImage: CIImage?

A CIImage object that encapsulates the operations configured in the filter.

**Required**

### Type Methods

static func customAttributes() -> [String : Any]?

Returns a dictionary that contains key-value pairs that describe the filter.

## Relationships

### Inherited By

- CIAffineClamp
- CIAffineTile
- CIAreaReductionFilter
- CIAttributedTextImageGenerator
- CIAztecCodeGenerator
- CIBarcodeGenerator
- CIBicubicScaleTransform
- CIBlendWithMask
- CIBloom
- CIBlurredRectangleGenerator
- CIBokehBlur
- CIBoxBlur
- CIBumpDistortion
- CIBumpDistortionLinear
- CICMYKHalftone
- CICannyEdgeDetector
- CICheckerboardGenerator
- CICircleSplashDistortion
- CICircularScreen
- CICircularWrap
- CICode128BarcodeGenerator
- CIColorAbsoluteDifference
- CIColorClamp
- CIColorControls
- CIColorCrossPolynomial
- CIColorCube
- CIColorCubeWithColorSpace
- CIColorCubesMixedWithMask
- CIColorCurves
- CIColorInvert
- CIColorMap
- CIColorMatrix
- CIColorMonochrome
- CIColorPolynomial
- CIColorPosterize
- CIColorThreshold
- CIColorThresholdOtsu
- CIComicEffect
- CICompositeOperation
- CIConvertLab
- CIConvolution
- CICoreMLModel
- CICrystallize
- CIDepthOfField
- CIDepthToDisparity
- CIDiscBlur
- CIDisparityToDepth
- CIDisplacementDistortion
- CIDither
- CIDocumentEnhancer
- CIDotScreen
- CIDroste
- CIEdgePreserveUpsample
- CIEdgeWork
- CIEdges
- CIEightfoldReflectedTile
- CIExposureAdjust
- CIFalseColor
- CIFourCoordinateGeometryFilter
- CIFourfoldReflectedTile
- CIFourfoldRotatedTile
- CIFourfoldTranslatedTile
- CIGaborGradients
- CIGammaAdjust
- CIGaussianBlur
- CIGaussianGradient
- CIGlassDistortion
- CIGlassLozenge
- CIGlideReflectedTile
- CIGloom
- CIHatchedScreen
- CIHeightFieldFromMask
- CIHexagonalPixellate
- CIHighlightShadowAdjust
- CIHistogramDisplay
- CIHoleDistortion
- CIHueAdjust
- CIHueSaturationValueGradient
- CIKaleidoscope
- CILabDeltaE
- CILanczosScaleTransform
- CILenticularHaloGenerator
- CILightTunnel
- CILineOverlay
- CILineScreen
- CILinearGradient
- CILinearToSRGBToneCurve
- CIMaskToAlpha
- CIMaskedVariableBlur
- CIMaximumComponent
- CIMaximumScaleTransform
- CIMedian
- CIMeshGenerator
- CIMinimumComponent
- CIMix
- CIMorphologyGradient
- CIMorphologyMaximum
- CIMorphologyMinimum
- CIMorphologyRectangleMaximum
- CIMorphologyRectangleMinimum
- CIMotionBlur
- CINinePartStretched
- CINinePartTiled
- CINoiseReduction
- CIOpTile
- CIPDF417BarcodeGenerator
- CIPaletteCentroid
- CIPalettize
- CIParallelogramTile
- CIPersonSegmentation
- CIPerspectiveRotate
- CIPerspectiveTile
- CIPhotoEffect
- CIPinchDistortion
- CIPixellate
- CIPointillize
- CIQRCodeGenerator
- CIRadialGradient
- CIRandomGenerator
- CIRoundedRectangleGenerator
- CIRoundedRectangleStrokeGenerator
- CISRGBToneCurveToLinear
- CISaliencyMap
- CISepiaTone
- CIShadedMaterial
- CISharpenLuminance
- CISixfoldReflectedTile
- CISixfoldRotatedTile
- CISmoothLinearGradient
- CISobelGradients
- CISpotColor
- CISpotLight
- CIStarShineGenerator
- CIStraighten
- CIStretchCrop
- CIStripesGenerator
- CISunbeamsGenerator
- CITemperatureAndTint
- CITextImageGenerator
- CIThermal
- CIToneCurve
- CIToneMapHeadroom
- CITorusLensDistortion
- CITransitionFilter
- CITriangleKaleidoscope
- CITriangleTile
- CITwelvefoldReflectedTile
- CITwirlDistortion
- CIUnsharpMask
- CIVibrance
- CIVignette
- CIVignetteEffect
- CIVortexDistortion
- CIWhitePointAdjust
- CIXRay
- CIZoomBlur

## See Also

### Configuring Type-Safe Filters

Blur Filters

Color Adjustment Filters

Color Effect Filters

Composite Operations

Convolution Filters

Distortion Filters

Generator Filters

Geometry Adjustment Filters

Gradient Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

