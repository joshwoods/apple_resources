

- TabularData
- DiscontiguousColumnSlice
-  trimPrefix(while:) 

Instance Method

# trimPrefix(while:)

TabularDataSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func trimPrefix(while predicate: (Self.Element) throws -> Bool) throws
```

Available when `Self` is `Self.SubSequence`.

