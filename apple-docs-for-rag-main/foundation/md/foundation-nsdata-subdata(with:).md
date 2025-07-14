

- Foundation
- NSData
-  subdata(with:) 

Instance Method

# subdata(with:)

Returns a new data object containing the data object’s bytes that fall within the limits specified by a given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func subdata(with range: NSRange) -> Data
```

## Parameters 

`range`  

The range in the receiver from which to get the data. If this range is not within the data object’s range of bytes, rangeException is raised.

## Return Value

A data object containing the receiver’s bytes that fall within the limits specified by `range`.

## Discussion

A sample using this method can be found in Working With Binary Data.

## See Also

### Finding Data

func range(of: Data, options: NSData.SearchOptions, in: NSRange) -> NSRange

Finds and returns the range of the first occurrence of the given data, within the given range, subject to given options.

struct SearchOptions

Options for method used to search data objects.

