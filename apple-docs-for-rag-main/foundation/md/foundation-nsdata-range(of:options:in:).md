

- Foundation
- NSData
-  range(of:options:in:) 

Instance Method

# range(of:options:in:)

Finds and returns the range of the first occurrence of the given data, within the given range, subject to given options.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func range(
    of dataToFind: Data,
    options mask: NSData.SearchOptions = [],
    in searchRange: NSRange
) -> NSRange
```

## Parameters 

`dataToFind`  

The data for which to search.

`mask`  

A mask specifying search options. The NSData.SearchOptions options may be specified singly or by combining them with the C bitwise `OR` operator.

`searchRange`  

The range within the receiver in which to search for `dataToFind`. If this range is not within the data object’s range of bytes, rangeException is raised.

## Return Value

An NSRange structure giving the location and length of `dataToFind` within `searchRange`, modulo the options in `mask`. The range returned is relative to the start of the searched data, not the passed-in search range. Returns ``` {``NSNotFound``, 0} ``` if `dataToFind` is not found or is empty.

## See Also

### Finding Data

func subdata(with: NSRange) -> Data

Returns a new data object containing the data object’s bytes that fall within the limits specified by a given range.

struct SearchOptions

Options for method used to search data objects.

