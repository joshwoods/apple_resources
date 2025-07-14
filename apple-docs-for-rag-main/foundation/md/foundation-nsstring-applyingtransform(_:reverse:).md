

- Foundation
- NSString
-  applyingTransform(\_:reverse:) 

Instance Method

# applyingTransform(\_:reverse:)

Returns a new string by applying a specified transform to the string.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func applyingTransform(
    _ transform: StringTransform,
    reverse: Bool
) -> String?
```

## Discussion

You can use this method to, for example, transliterate text from one script to another, strip diacritics or combining marks, and get the unicode names of characters.

Note

The constants defined by the StringTransform type offer a subset of the functionality provided by the underlying ICU transform functionality. To apply an ICU transform defined in the ICU User Guide that doesn’t have a corresponding StringTransform constant, create an instance of NSMutableString and call the applyTransform(_:reverse:range:updatedRange:) method instead.

.

## See Also

### Related Documentation

func applyTransform(StringTransform, reverse: Bool, range: NSRange, updatedRange: NSRangePointer?) -> Bool

Transliterates the receiver by applying a specified ICU string transform.

### Transforming Strings

struct StringTransform

Constants representing an ICU string transform.

