

- Swift
- String
-  utf8CString 

Instance Property

# utf8CString

A contiguously stored null-terminated UTF-8 representation of the string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var utf8CString: ContiguousArray { get }
```

## Discussion

To access the underlying memory, invoke `withUnsafeBufferPointer` on the array.

```
let s = "Hello!"
let bytes = s.utf8CString
print(bytes)
// Prints "[72, 101, 108, 108, 111, 33, 0]"

bytes.withUnsafeBufferPointer { ptr in
    print(strlen(ptr.baseAddress!))
}
// Prints "6"
```

## See Also

### Getting C Strings

func withCString&lt;Result>((UnsafePointer&lt;Int8>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the string, represented as a null-terminated sequence of UTF-8 code units.

func withCString&lt;Result, TargetEncoding>(encodedAs: TargetEncoding.Type, (UnsafePointer&lt;TargetEncoding.CodeUnit>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the string, represented as a null-terminated sequence of code units.

