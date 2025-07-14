

- Swift
- String
-  isContiguousUTF8 

Instance Property

# isContiguousUTF8

Returns whether this string is capable of providing access to validly-encoded UTF-8 contents in contiguous memory in O(1) time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isContiguousUTF8: Bool { get }
```

## Discussion

Contiguous strings always operate in O(1) time for withUTF8 and always give a result for String.UTF8View.withContiguousStorageIfAvailable. Contiguous strings also benefit from fast-paths and better optimizations.

## See Also

### Working with Encodings

static var availableStringEncodings: [String.Encoding]

An array of the encodings that strings support in the application’s environment.

static var defaultCStringEncoding: String.Encoding

The C-string encoding assumed for any method accepting a C string as an argument.

static func localizedName(of: String.Encoding) -> String

Returns a human-readable string giving the name of the specified encoding.

func makeContiguousUTF8()

If this string is not contiguous, make it so. If this mutates the string, it will invalidate any pre-existing indices.

func withUTF8&lt;R>((UnsafeBufferPointer&lt;UInt8>) throws -> R) rethrows -> R

Runs `body` over the content of this string in contiguous memory. If this string is not contiguous, this will first make it contiguous, which will also speed up subsequent access. If this mutates the string, it will invalidate any pre-existing indices.

