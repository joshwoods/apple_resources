

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXSelectedTextRangesAttribute 

Global Variable

# kAXSelectedTextRangesAttribute

macOS 10.5+

``` source
var kAXSelectedTextRangesAttribute: String { get }
```

## Discussion

An array of noncontiguous ranges of characters (not bytes) that defines the current selections of an editable text element.

Value: A CFArrayRef of kAXValueCFRanges.

Writable? Yes.

Recommended for text elements that support noncontiguous selections.

