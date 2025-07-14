

- Quartz
- Quartz Composer
- QCPlugIn
-  Pixel Formats 

API Collection

# Pixel Formats

Supported image pixel formats.

## Topics

### Constants

let QCPlugInPixelFormatARGB8: String

An ARGB8 format. The alpha component is stored in the most significant bits of each pixel. Each pixel component is 8 bits. For best performance, use this format on PowerPC-based Macintosh computers, as it represents of the order of the data in memory.

Deprecated

let QCPlugInPixelFormatBGRA8: String

A BGRA8 format. The alpha component is stored in the least significant bits of each pixel. Each pixel component is 8 bits. For best performance, use this format on Intel-PC-based Macintosh computers, as it represents of the order of the data in memory.

Deprecated

let QCPlugInPixelFormatRGBAf: String

An RGBAf format. Pixel components are represented as floating-point values.

Deprecated

let QCPlugInPixelFormatI8: String

An I8 format. Intensity information is represented as an 8-bit value.

Deprecated

let QCPlugInPixelFormatIf: String

An If format. Intensity information is represented as a floating-point value.

Deprecated

## See Also

### Constants

Patch Attributes

Attributes for custom patches.

Input and Output Port Attributes

Attributes for input and output ports.

Port Input and Output Types

Data types for input and output ports.

Execution Arguments

Arguments to the method execute(_:atTime:withArguments:).

struct QCPlugInExecutionMode

Execution modes for custom patches.

Deprecated

struct QCPlugInTimeMode

Time modes for custom patches.

Deprecated

