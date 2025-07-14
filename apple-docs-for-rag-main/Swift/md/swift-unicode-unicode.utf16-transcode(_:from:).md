

- Swift
- Unicode
- Unicode.UTF16
-  transcode(\_:from:) 

Type Method

# transcode(\_:from:)

Converts a scalar from another encoding’s representation, returning `nil` if the scalar can’t be represented in this encoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func transcode(
    _ content: FromEncoding.EncodedScalar,
    from _: FromEncoding.Type
) -> Unicode.UTF16.EncodedScalar? where FromEncoding : _UnicodeEncoding
```

## Discussion

A default implementation of this method will be provided automatically for any conforming type that does not implement one.

