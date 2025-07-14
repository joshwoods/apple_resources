

- Core Video
- CVBuffer
-  CVBuffer Attachment Keys 

API Collection

# CVBuffer Attachment Keys

The attachment types for a Core Video buffer.

## Topics

### Constants

let kCVBufferMovieTimeKey: CFString

The movie time associated with the buffer. Generally only available for frames emitted by QuickTime (type `CFDictionary` containing the kCVBufferTimeValueKey and kCVBufferTimeScaleKey keys).

let kCVBufferTimeValueKey: CFString

The time value associated with the movie.

let kCVBufferTimeScaleKey: CFString

The time scale associated with the movie.

## See Also

### Constants

CVBuffer Attribute Keys

The attributes associated with Core Video buffers.

