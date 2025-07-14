

- Foundation
- URL
-  URL.AsyncBytes 

Structure

# URL.AsyncBytes

An asynchronous sequence of bytes loaded from the URL.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AsyncBytes
```

## Topics

### Adapting Textual Sequences

var lines: AsyncLineSequence&lt;URL.AsyncBytes>

The URL’s resource data, as an asynchronous sequence of lines of text.

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Loading URL contents asynchronously

var resourceBytes: URL.AsyncBytes

The URL’s resource data, as an asynchronous sequence of bytes.

var lines: AsyncLineSequence&lt;URL.AsyncBytes>

The URL’s resource data, as an asynchronous sequence of lines of text.

