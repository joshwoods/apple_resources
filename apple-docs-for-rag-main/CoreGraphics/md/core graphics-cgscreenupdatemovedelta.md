

- Core Graphics
-  CGScreenUpdateMoveDelta 

Structure

# CGScreenUpdateMoveDelta

The distance, in pixel units, that an onscreen region moves.

Mac CatalystmacOS

``` source
struct CGScreenUpdateMoveDelta
```

## Overview

Move operation notifications are restricted to changes that move a region by an integer number of pixels. The fields `dX` and `dY` describe the direction of movement:

- Positive values of `dX` indicate movement to the right.

- Negative values of `dX` indicate movement to the left.

- Positive values of `dY` indicate movement downward.

- Negative values of `dY` indicate movement upward.

## Topics

### Initializers

init()

init(dX: Int32, dY: Int32)

### Instance Properties

var dX: Int32

var dY: Int32

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

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

struct CGScreenUpdateOperation

Types of screen-update operations.

struct CGWindowImageOption

The data type to use to specify the type of image to be generated for a window.

struct CGWindowListOption

The data type used to specify the options for gathering a list of windows.

struct CGColorBufferFormat

struct CGColorDataFormat

struct CGPDFAccessPermissions

struct CGPSConverterCallbacks

A structure for holding the callbacks provided when you create a PostScript converter object.

