

- AppKit
- NSTextFinderClient
-  stringLength() 

Instance Method

# stringLength()

Returns the full length of the conceptually concatenated string return by the `stringAtIndex:effectiveRange:endsWithSearchBoundary:` method.

macOS

``` source
optional func stringLength() -> Int
```

## Return Value

Returns the full length of the conceptually concatenated string in the second model, that is, the sum of the lengths of all of its substrings.

## Discussion

See NSTextFinder for more information.

## See Also

### String Searching

var string: String

Allows the client to specify a single string for searching.

func string(at: Int, effectiveRange: NSRangePointer, endsWithSearchBoundary: UnsafeMutablePointer&lt;ObjCBool>) -> String

Returns the found string that is created by conceptually mapping its content to a single string, which is composed of a concatenation of all its substrings.

