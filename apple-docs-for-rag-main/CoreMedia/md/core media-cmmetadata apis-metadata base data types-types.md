

- Core Media
- CMMetadata APIs
-  Metadata Base Data Types 

API Collection

# Metadata Base Data Types

Constants that describe metadata base data types.

## Topics

### Constants

let kCMMetadataBaseDataType_RawData: CFString

A sequence of bytes whose interpretation based upon an agreement between the reader and the writer.

let kCMMetadataBaseDataType_UTF8: CFString

UTF-8 string.

let kCMMetadataBaseDataType_UTF16: CFString

UTF-16 string.

let kCMMetadataBaseDataType_GIF: CFString

GIF image.

let kCMMetadataBaseDataType_JPEG: CFString

JPEG image.

let kCMMetadataBaseDataType_PNG: CFString

PNG image.

let kCMMetadataBaseDataType_BMP: CFString

BMP image.

let kCMMetadataBaseDataType_Float32: CFString

32-bit big endian floating point number.

let kCMMetadataBaseDataType_Float64: CFString

64-bit big endian floating point number.

let kCMMetadataBaseDataType_SInt8: CFString

8-bit signed integer.

let kCMMetadataBaseDataType_SInt16: CFString

16-bit big endian signed integer.

let kCMMetadataBaseDataType_SInt32: CFString

32-bit big endian signed integer.

let kCMMetadataBaseDataType_SInt64: CFString

64-bit big endian signed integer.

let kCMMetadataBaseDataType_UInt8: CFString

8-bit unsigned integer.

let kCMMetadataBaseDataType_UInt16: CFString

16-bit big endian unsigned integer.

let kCMMetadataBaseDataType_UInt32: CFString

32-bit big endian unsigned integer.

let kCMMetadataBaseDataType_UInt64: CFString

64-bit big endian unsigned integer.

let kCMMetadataBaseDataType_PointF32: CFString

Consists of two 32-bit big endian floating point values, the x and y values, respectively.

let kCMMetadataBaseDataType_DimensionsF32: CFString

Consists of a 32-bit big endian floating point x value followed by a 32-bit floating point y value.

let kCMMetadataBaseDataType_RectF32: CFString

Consists of four 32-bit big endian floating point values, the origin’s x, origin’s y, width and height values, respectively. May also be interpreted as a 32-bit floating point origin followed by a 32-bit floating point dimension.

let kCMMetadataBaseDataType_AffineTransformF64: CFString

A type that identifies a 3x3 matrix of 64-bit big endian floating point numbers in a row-major order that specify an affine transform.

let kCMMetadataBaseDataType_PerspectiveTransformF64: CFString

A 3x3 matrix of 64-bit big endian floating point numbers the system stores in row-major order that specify a perspective transform.

let kCMMetadataBaseDataType_PolygonF32: CFString

Three or more pairs of 32-bit floating point numbers (x and y values) that define the vertices of a polygon.

let kCMMetadataBaseDataType_PolylineF32: CFString

Two or more pairs of 32-bit floating point numbers (x and y values) that define a multi-segmented line.

let kCMMetadataBaseDataType_JSON: CFString

UTF-8 encoded JSON data.

## See Also

### Constants

Metadata Identifier Error Codes

Error codes that indicate metadata identifier errors.

Metadata Registry Error Codes

Error codes that indicate metadata registry errors.

Metadata Identifier Keyspaces

Constants that describe metadata identifier keyspaces.

Metadata Identifiers

Constants that describe metadata identifiers.

Metadata Data Types

Constants that describe metadata data types.

