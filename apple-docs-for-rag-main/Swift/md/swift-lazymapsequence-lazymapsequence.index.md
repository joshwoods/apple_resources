

- Swift
- LazyMapSequence
-  LazyMapSequence.Index 

Type Alias

# LazyMapSequence.Index

A type that represents a position in the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias Index = Base.Index
```

Available when `Base` conforms to `Collection`.

## Discussion

Valid indices consist of the position of every element and a “past the end” position that’s not valid for use as a subscript argument.

