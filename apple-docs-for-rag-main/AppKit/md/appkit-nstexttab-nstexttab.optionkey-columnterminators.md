

- AppKit
- NSTextTab
- NSTextTab.OptionKey
-  columnTerminators 

Type Property

# columnTerminators

The value is an `NSCharacterSet` object.

macOS 10.0+

``` source
static let columnTerminators: NSTextTab.OptionKey
```

## Discussion

The character set is used to determine the terminating character for a tab column. The tab and newline characters are implied even if they don’t exist in the character set. This attribute is optional.

