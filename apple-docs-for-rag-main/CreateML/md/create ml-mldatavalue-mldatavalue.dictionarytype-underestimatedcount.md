

- Create ML
- MLDataValue
- MLDataValue.DictionaryType
-  underestimatedCount 

Instance Property

# underestimatedCount

A value less than or equal to the number of elements in the collection.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var underestimatedCount: Int { get }
```

## Discussion

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

