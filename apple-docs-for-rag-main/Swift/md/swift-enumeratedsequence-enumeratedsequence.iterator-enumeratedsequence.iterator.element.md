

- Swift
- EnumeratedSequence
- EnumeratedSequence.Iterator
-  EnumeratedSequence.Iterator.Element 

Type Alias

# EnumeratedSequence.Iterator.Element

The type of element returned by `next()`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias Element = (offset: Int, element: Base.Element)
```

Available when `Base` conforms to `Sequence`.

