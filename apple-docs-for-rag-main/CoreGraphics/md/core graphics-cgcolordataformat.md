

- Core Graphics
-  CGColorDataFormat 

Structure

# CGColorDataFormat

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGColorDataFormat
```

## Topics

### Initializers

init()

init(version: UInt32, colorspace_info: Unmanaged&lt;CFTypeRef>!, bitmap_info: CGBitmapInfo, bits_per_component: Int, bytes_per_row: Int, intent: CGColorRenderingIntent, decode: UnsafeMutablePointer&lt;CGFloat>!)

### Instance Properties

var bitmap_info: CGBitmapInfo

var bits_per_component: Int

var bytes_per_row: Int

var colorspace_info: Unmanaged&lt;CFTypeRef>!

var decode: UnsafeMutablePointer&lt;CGFloat>!

var intent: CGColorRenderingIntent

var version: UInt32

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

class CGPSConverter

An opaque data type used to convert PostScript data to PDF data.

struct CGCaptureOptions

Configuration parameters that are used when capturing displays.

struct CGConfigureOption

The scope of the changes in a display configuration transaction.

struct CGDeviceColor

struct CGDisplayChangeSummaryFlags

The configuration parameters that are passed to a display reconfiguration callback function.

struct CGEventFilterMask

Specify masks for classes of low-level events that can be filtered during event suppression states.

struct CGEventFlags

Constants that indicate the modifier key state at the time an event is created, as well as other event-related states.

typealias CGEventTapInformation

Defines the structure used to report information about event taps.

struct CGScreenUpdateMoveDelta

The distance, in pixel units, that an onscreen region moves.

struct CGScreenUpdateOperation

Types of screen-update operations.

struct CGWindowImageOption

The data type to use to specify the type of image to be generated for a window.

struct CGWindowListOption

The data type used to specify the options for gathering a list of windows.

struct CGColorBufferFormat

struct CGPDFAccessPermissions

struct CGPSConverterCallbacks

A structure for holding the callbacks provided when you create a PostScript converter object.

