

- Swift
- String
- String.UTF8View
-  startIndex 

Instance Property

# startIndex

The position of the first code unit if the UTF-8 view is nonempty.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var startIndex: String.UTF8View.Index { get }
```

## Discussion

If the UTF-8 view is empty, `startIndex` is equal to `endIndex`.

