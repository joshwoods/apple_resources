

- Core Image
- CIFilter
-  RAW Image Options 

API Collection

# RAW Image Options

Options for creating a `CIFilter` object from RAW image data.

## Overview

You can also use the key kCIInputEVKey for RAW images.

## Topics

### Constants

static let decoderVersion: CIRAWFilterOption

A key for the version number of the method to be used for decoding. A newly initialized object defaults to the newest available decoder version for the given image type. You can request an alternative, older version to maintain compatibility with older releases. Must be one of the values listed for the supportedDecoderVersions key, otherwise a `nil` output image is generated. The associated value must be an `NSNumber` object that specifies an integer value in range of `0` to the current decoder version. When you request a specific version of the decoder, Core Image produces an image that is *visually* the same across different versions of the operating system. Core Image, however, does not guarantee that the same bits are produced across different versions of the operating system. That’s because the rounding behavior of floating-point arithmetic can vary due to differences in compilers or hardware. Note that this option has no effect if the image used for initialization is not RAW.

Deprecated

static let supportedDecoderVersions: CIRAWFilterOption

A key for the supported decoder versions. The associated value is an NSArray object that contains all supported decoder versions for the given image type, sorted in increasingly newer order. Each entry is an NSDictionary object that contains key-value pairs. All entries represent a valid version identifier that can be passed as the `kCIDecoderVersion` value for the key `kCIDecoderMethodKey`. Version values are read-only; attempting to set this value raises an exception. Currently, the only defined key is `@"version"` which has as its value an NSString that uniquely describing a given decoder version. This string might not be suitable for user interface display..

Deprecated

static let boostAmount: CIRAWFilterOption

A key for the amount of boost to apply to an image. The associated value is a floating-point value packaged as an NSNumber object. The value must be in the range of `0...1`. A value of `0` indicates no boost, that is, a linear response. The default value is `1`, which indicates full boost.

Deprecated

static let neutralChromaticityX: CIRAWFilterOption

The x value of the chromaticity. The associated value is a floating-point value packaged as an NSNumber object. You can query this value to get the current x value for neutral x, y.

Deprecated

static let neutralChromaticityY: CIRAWFilterOption

The y value of the chromaticity. The associated value is a floating-point value packaged as an NSNumber object. You can query this value to get the current y value for neutral x, y.

Deprecated

static let neutralTemperature: CIRAWFilterOption

A key for neutral temperature. The associated value is a floating-point value packaged as an NSNumber object. You can query this value to get the current temperature value.

Deprecated

static let neutralTint: CIRAWFilterOption

A key for the neutral tint. The associated value is a floating-point value packaged as an NSNumber object. Use this key to set or fetch the temperature and tint values. You can query this value to get the current tint value.

Deprecated

static let neutralLocation: CIRAWFilterOption

A key for the neutral position. Use this key to set the location in geometric coordinates of the unrotated output image that should be used as neutral. You cannot query this value; it is undefined for reading. The associated value is a two-element CIVector object that specifies the location (`x`, `y`).

Deprecated

static let scaleFactor: CIRAWFilterOption

A key for the scale factor. The associated value is a floating-point value packaged as an NSNumber object that specifies the desired scale factor at which the image will be drawn. Setting this value can greatly improve the drawing performance. A value of `1` is the identity. In some cases, if you change the scale factor and enable draft mode, performance can decrease. See allowDraftMode.

Deprecated

static let allowDraftMode: CIRAWFilterOption

A key for allowing draft mode. The associated value is a Boolean value packaged as an NSNumber object. It’s best not to use draft mode if the image needs to be drawn without draft mode at a later time, because changing the value from `true` to `false` is an expensive operation. If the optional scale factor is smaller than a certain value, additionally setting draft mode can improve image decoding speed without any perceivable loss of quality. However, turning on draft mode does not have any effect if the scale factor is not below this threshold.

Deprecated

static let ignoreImageOrientation: CIRAWFilterOption

A key for specifying whether to ignore the image orientation. The associated value is a Boolean value packaged as an NSNumber object. The default value is `false`. An image is usually loaded in its proper orientation, as long as the associated metadata records its orientation. For special purposes you might want to load the image in its physical orientation. The exact meaning of "physical orientation” is dependent on the specific image.

Deprecated

static let imageOrientation: CIRAWFilterOption

A key for the image orientation. The associated value is an integer value packaged as an NSNumber object. Valid values are in range `1...8` and follow the EXIF specification. The value is disregarded when the `kCIIgnoreImageOrientationKey` flag is set. You can change the orientation of the image by overriding this value. By changing this value you can rotate an image in 90-degree increments.

Deprecated

static let enableSharpening: CIRAWFilterOption

A key for the sharpening state. The associated value must be an NSNumber object that specifies a `BOOL` value (`true` or `false`). The default is `true`. This option has no effect if the image used for initialization is not RAW.

Deprecated

static let enableChromaticNoiseTracking: CIRAWFilterOption

A key for progressive chromatic noise tracking (based on ISO and exposure time). The associated value must be an NSNumber object that specifies a `BOOL` value (`true` or `false`). The default is `true`. This option has no effect if the image used for initialization is not RAW.

Deprecated

static let noiseReductionAmount: CIRAWFilterOption

A key for the amount to reduce noise in the image. The associated value must be an NSNumber object that specifies a floating-point value between `0.0` and `1.0`. The value has no effect if the image used for initialization is not RAW.

Deprecated

static let enableVendorLensCorrection: CIRAWFilterOption

A key for whether to automatically correct for image distortion from known lenses.

Deprecated

static let luminanceNoiseReductionAmount: CIRAWFilterOption

A key for the amount of noise reduction to apply to luminance data in the image.

Deprecated

static let colorNoiseReductionAmount: CIRAWFilterOption

A key for the amount of noise reduction to apply to color data in the image.

Deprecated

static let noiseReductionSharpnessAmount: CIRAWFilterOption

A key for the amount of sharpness enhancement to apply during noise reduction.

Deprecated

static let noiseReductionContrastAmount: CIRAWFilterOption

A key for the amount of contrast enhancement to apply during noise reduction.

Deprecated

static let noiseReductionDetailAmount: CIRAWFilterOption

A key for the amount of detail enhancement to apply during noise reduction.

Deprecated

static let boostShadowAmount: CIRAWFilterOption

A key for the amount to boost the shadow areas of the image. The associated value must be an NSNumber object that specifies floating-point value. The value has no effect if the image used for initialization is not RAW.

Deprecated

let kCIInputBiasKey: String

A key for the simple bias value to use along with the exposure adjustment (kCIInputEVKey). The associated value must be an NSNumber object that specifies floating-point value. The value has no effect if the image used for initialization is not RAW.

static let linearSpaceFilter: CIRAWFilterOption

A key for the filter to apply to the image while it is temporarily in a linear color space as part of RAW image processing. The associated value must be a `CIFilter` object.

Deprecated

static let outputNativeSize: CIRAWFilterOption

A key for the full native size of the original, non-transformed RAW image. The associated value is a CIVector object whose X and Y values are the image’s width and height. This key is read-only.

Deprecated

static let activeKeys: CIRAWFilterOption

A key for the set of input keys available for use. The associated value is an NSSet object containing the set of input keys which may be used to affect the output image. (Depending on the input image type and the decoder version, some input keys may be unavailable.) This key is read-only.

Deprecated

