

- AppKit
- NSTextFinderClient
-  string 

Instance Property

# string

Allows the client to specify a single string for searching.

macOS

``` source
optional var string: String { get }
```

## Discussion

If the client cannot logically or efficiently flatten itself into a single string, then the string(at:effectiveRange:endsWithSearchBoundary:) and stringLength() methods should be implemented instead.

## See Also

### String Searching

func string(at: Int, effectiveRange: NSRangePointer, endsWithSearchBoundary: UnsafeMutablePointer&lt;ObjCBool>) -> String

Returns the found string that is created by conceptually mapping its content to a single string, which is composed of a concatenation of all its substrings.

func stringLength() -> Int

Returns the full length of the conceptually concatenated string return by the `stringAtIndex:effectiveRange:endsWithSearchBoundary:` method.

