

- Swift
- String
- String.UnicodeScalarView
-  startIndex 

Instance Property

# startIndex

The position of the first Unicode scalar value if the string is nonempty.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var startIndex: String.UnicodeScalarView.Index { get }
```

## Discussion

If the string is empty, `startIndex` is equal to `endIndex`.

