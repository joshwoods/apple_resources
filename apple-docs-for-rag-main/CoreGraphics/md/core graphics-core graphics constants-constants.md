

- Core Graphics
-  Core Graphics Constants 

API Collection

# Core Graphics Constants

## Topics

### Constants

class let colorSpace: CFString

This key specifies the color space of the output buffer. If this key is not included in the dictionary, the output buffer uses the same color space as the display. The value associated with this key must be a CGColorSpace for the desired color space.

Deprecated

class let conversionBlackPointCompensation: CFString

An option for whether to apply black point compensation when converting between color profiles.

var kCGDisplayBitsPerPixel: String

Specifies a CFNumber integer value that represents the number of bits in a pixel.

var kCGDisplayBitsPerSample: String

Specifies a CFNumber integer value that represents the number of bits in an individual sample (for example, a color value in an RGB pixel).

var kCGDisplayBlendNormal: Double

The blend color is not applied at the start or end of a fade operation.

var kCGDisplayBlendSolidColor: Double

The user sees only the blend color at the start or end of a fade operation.

var kCGDisplayBytesPerRow: String

Specifies a CFNumber integer value that represents the number of bytes in a row on the display.

var kCGDisplayFadeReservationInvalidToken: Int32

var kCGDisplayHeight: String

Specifies a CFNumber integer value that represents the height of the display in pixels.

var kCGDisplayIOFlags: String

Specifies a CFNumber integer value that contains the I/O Kit display mode flags. For more information, see the header file `IOKit/IOGraphicsTypes.h`.

var kCGDisplayMode: String

Specifies a `CFNumber` integer value that represents the I/O Kit display mode number.

var kCGDisplayModeIsInterlaced: String

Specifies a CFBoolean value indicating that the I/O Kit interlace mode flag is set.

var kCGDisplayModeIsSafeForHardware: String

Specifies a CFBoolean value indicating that the display mode doesn’t need a confirmation dialog to be set.

Deprecated

var kCGDisplayModeIsStretched: String

Specifies a CFBoolean value indicating that the I/O Kit stretched mode flag is set.

var kCGDisplayModeIsTelevisionOutput: String

Specifies a CFBoolean value indicating that the I/O Kit television output mode flag is set.

var kCGDisplayModeUsableForDesktopGUI: String

Specifies a CFBoolean value that indicates whether the display is suitable for use with the macOS graphical user interface. The criteria include factors such as sufficient width and height and adequate pixel depth.

var kCGDisplayRefreshRate: String

Specifies a `CFNumber` double-precision floating point value that represents the refresh rate of a CRT display.

var kCGDisplaySamplesPerPixel: String

Specifies a CFNumber integer value that represents the number of samples in a pixel.

let kCGDisplayShowDuplicateLowResolutionModes: CFString

class let destinationRect: CFString

This key specifies that the display stream outputs the frame data into a subset of the output `IOSurface` object.

Deprecated

class let minimumFrameTime: CFString

This key specifies the desired minimum time between frame updates, allowing you to throttle the rate at which updates are received. If this key is not included in the dictionary, the default value is `0`, meaning that updates are not throttled. The value must be specified as a `CFNumber`.

Deprecated

class let queueDepth: CFString

This key specifies the number of frames to keep in the queue. If this key is not included in the dictionary, the default value is `3` frames. Specifying more frames uses more memory, but may allow you to process frame data without stalling the display stream. The value associated with this key should be specified as a `CFNumber`, and should not exceed `8` frames.

Deprecated

class let showCursor: CFString

This key specifies whether the cursor should appear in the stream. If this key is not included in the dictionary, the cursor is visible. The value must be specified as a `CFBoolean`.

Deprecated

class let sourceRect: CFString

This key specifies that the display stream only samples a subset of the display’s framebuffer.

Deprecated

class let yCbCrMatrix: CFString

This key should only be included if you the display stream is creating output frames in either the 420v or 420f formats. It is used to specify the YCbCr matrix applied to the output surface.

Deprecated

class let yCbCrMatrix_ITU_R_601_4: CFString

Specifies the YCbCr to RGB conversion matrix for standard digital television (ITU R 601) images.

class let yCbCrMatrix_ITU_R_709_2: CFString

Specifies the YCbCr to RGB conversion matrix for HDTV digital television (ITU R 709) images.

class let yCbCrMatrix_SMPTE_240M_1995: CFString

Specifies the YCbCR to RGB conversion matrix for 1920 x 1135 HDTV (SMPTE 240M 1995).

var kCGDisplayWidth: String

Specifies a CFNumber integer value that represents the width of the display in pixels.

Deprecated

let kCGFontIndexInvalid: CGFontIndex

An invalid font index (a value which never represents a valid glyph).

let kCGFontIndexMax: CGFontIndex

The maximum allowed value of a CGFontIndex.

let kCGGlyphMax: CGFontIndex

The maximum allowed value of a CGGlyph.

var kCGIODisplayModeID: String

var kCGMouseDownEventMaskingDeadSwitchTimeout: Double

var kCGNotifyEventTapAdded: String

var kCGNotifyEventTapRemoved: String

var kCGNotifyGUIConsoleSessionChanged: String

var kCGNotifyGUISessionUserChanged: String

var kCGNumReservedWindowLevels: Int32

var kCGSessionConsoleSetKey: String

A `CFNumber` 32-bit unsigned integer value that represents a set of hardware composing a console.

var kCGSessionLoginDoneKey: String

A `CFBoolean` value indicating whether the login operation has been done.

var kCGSessionOnConsoleKey: String

A `CFBoolean` value indicating whether the session is on a console.

var kCGSessionUserIDKey: String

A `CFNumber` 32-bit unsigned integer value that encodes a user ID for the session’s current user.

var kCGSessionUserNameKey: String

A `CFString` value that encodes the session’s short user name as set by the login operation.

let kCGWindowAlpha: CFString

let kCGWindowBackingLocationVideoMemory: CFString

let kCGWindowBounds: CFString

let kCGWindowIsOnscreen: CFString

let kCGWindowLayer: CFString

let kCGWindowMemoryUsage: CFString

let kCGWindowName: CFString

let kCGWindowNumber: CFString

let kCGWindowOwnerName: CFString

let kCGWindowOwnerPID: CFString

let kCGWindowSharingState: CFString

let kCGWindowStoreType: CFString

let CGPointZero: CGPoint

A point constant with location `(0,0)`. The zero point is equivalent to `CGPointMake(0,0)`.

let CGRectZero: CGRect

A rectangle constant with location `(0,0)`, and width and height of 0. The zero rectangle is equivalent to `CGRectMake(0,0,0,0)`.

let CGSizeZero: CGSize

A size constant with width and height of `0`. The zero size is equivalent to `CGSizeMake(0,0)`.

let kCGWindowWorkspace: CFStringDeprecated

class let preserveAspectRatio: CFString

This key specifies whether the display stream preserves the aspect ratio of the source pixel data. If this key is not included in the dictionary, then the aspect ratio is preserved. If the aspect ratio is preserved, then the display stream adds black bars to the output data. If the aspect ratio is not preserved, then the pixel data is stretched to fit the output buffer’s dimensions. The value associated with the key must be a `CFBoolean`.

Deprecated

var CG_HDR_BT_2100: Int32

let kCGBitmapByteOrder16Host: CGBitmapInfo

16-bit, host endian format.

let kCGBitmapByteOrder32Host: CGBitmapInfo

32-bit, host endian format.

let kCGColorSpaceExtendedRange: CFString

var kCGDefaultHDRImageContentHeadroom: Float

let kCGEXRToneMappingGammaDefog: CFString

let kCGEXRToneMappingGammaExposure: CFString

let kCGEXRToneMappingGammaKneeHigh: CFString

let kCGEXRToneMappingGammaKneeLow: CFString

var kCGNullDirectDisplay: CGDirectDisplayID

A value that will never correspond to actual hardware.

var kCGNullWindowID: CGWindowID

var kCGNumReservedBaseWindowLevels: Int32

let kCGPDFContextAccessPermissions: CFString

let kCGPDFContextCreateLinearizedPDF: CFString

let kCGPDFContextCreatePDFA: CFString

let kCGPDFOutlineChildren: CFString

let kCGPDFOutlineDestination: CFString

let kCGPDFOutlineDestinationRect: CFString

let kCGPDFOutlineTitle: CFString

let kCGSkipBoostToHDR: CFString

let kCGUse100nitsHLGOOTF: CFString

let kCGUseBT1886ForCoreVideoGamma: CFString

let kCGUseLegacyHDREcosystem: CFString

var kCGAssistiveTechHighWindowLevel: CGWindowLevel

var kCGBackstopMenuLevel: CGWindowLevel

var kCGDockWindowLevel: CGWindowLevel

var kCGDraggingWindowLevel: CGWindowLevel

var kCGFloatingWindowLevel: CGWindowLevel

var kCGHelpWindowLevel: CGWindowLevel

var kCGMainMenuWindowLevel: CGWindowLevel

var kCGModalPanelWindowLevel: CGWindowLevel

var kCGNormalWindowLevel: CGWindowLevel

var kCGOverlayWindowLevel: CGWindowLevel

var kCGPopUpMenuWindowLevel: CGWindowLevel

var kCGScreenSaverWindowLevel: CGWindowLevel

var kCGStatusWindowLevel: CGWindowLevel

var kCGTornOffMenuWindowLevel: CGWindowLevel

var kCGUtilityWindowLevel: CGWindowLevel

## See Also

### Reference

Core Graphics Structures

Core Graphics Enumerations

Core Graphics Functions

Core Graphics Data Types

