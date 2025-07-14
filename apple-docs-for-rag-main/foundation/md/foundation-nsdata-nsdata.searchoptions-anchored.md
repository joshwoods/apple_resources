

- Foundation
- NSData
- NSData.SearchOptions
-  anchored 

Type Property

# anchored

Search is limited to start (or end, if searching backwards) of the data object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var anchored: NSData.SearchOptions { get }
```

## Discussion

This option performs searching only on bytes at the beginning of the range (or the end when using backwards). No match at the beginning or end means nothing is found, even if a matching sequence of bytes occurs elsewhere in the data object.

## See Also

### Constants

static var backwards: NSData.SearchOptions

Search from the end of the data object.

static var backwards: NSData.SearchOptions

Search from the end of the data object.

