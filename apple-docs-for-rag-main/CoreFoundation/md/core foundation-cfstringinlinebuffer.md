

- Core Foundation
-  CFStringInlineBuffer 

Structure

# CFStringInlineBuffer

Defines the buffer and related fields used for in-line buffer access of characters in CFString objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFStringInlineBuffer
```

## Overview

This structure is used for in-line buffer access of characters contained by a CFString object. Use the CFStringInitInlineBuffer(_:_:_:) function for initializing the fields of this structure; do not do it manually. Once the buffer is initialized, use the CFStringGetCharacterFromInlineBuffer(_:_:) function to access characters from the buffer. Do not access the fields directly as they might change between releases.

The only reason this structure is not opaque is to allow the in-line functions to access its fields.

## Topics

### Initializers

init()

init(buffer: (UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar), theString: Unmanaged&lt;CFString>!, directUniCharBuffer: UnsafePointer&lt;UniChar>!, directCStringBuffer: UnsafePointer&lt;CChar>!, rangeToBuffer: CFRange, bufferedRangeStart: CFIndex, bufferedRangeEnd: CFIndex)

### Instance Properties

var buffer: (UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar, UniChar)

var bufferedRangeEnd: CFIndex

var bufferedRangeStart: CFIndex

var directCStringBuffer: UnsafePointer&lt;CChar>!

var directUniCharBuffer: UnsafePointer&lt;UniChar>!

var rangeToBuffer: CFRange

var theString: Unmanaged&lt;CFString>!

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

typealias CFStringEncoding

An integer type for constants used to specify supported string encodings in various CFString functions.

enum CFStringEncodings

Index type for constants used to specify external string encodings.

struct CFStringCompareFlags

A CFOptionFlags type for specifying options for string comparison .

