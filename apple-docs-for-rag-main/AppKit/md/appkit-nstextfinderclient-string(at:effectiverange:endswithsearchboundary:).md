

- AppKit
- NSTextFinderClient
-  string(at:effectiveRange:endsWithSearchBoundary:) 

Instance Method

# string(at:effectiveRange:endsWithSearchBoundary:)

Returns the found string that is created by conceptually mapping its content to a single string, which is composed of a concatenation of all its substrings.

macOS 10.0+

``` source
optional func string(
    at characterIndex: Int,
    effectiveRange outRange: NSRangePointer,
    endsWithSearchBoundary outFlag: UnsafeMutablePointer
) -> String
```

## Parameters 

`characterIndex`  

The given character index the client should return.

`outRange`  

Returns, by reference, the “effective range” of that substring in the full conceptually concatenated string

`outFlag`  

Returns, by-reference, whether the substring ends with a “search boundary”, meaning that NSTextFinder should not attempt to find any matches that overlap this boundary.

## Return Value

Returns the found string.

## Discussion

See NSTextFinder for more information.

## See Also

### String Searching

var string: String

Allows the client to specify a single string for searching.

func stringLength() -> Int

Returns the full length of the conceptually concatenated string return by the `stringAtIndex:effectiveRange:endsWithSearchBoundary:` method.

