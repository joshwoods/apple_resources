

- AppKit
- NSTextCheckingClient
-  view(for:firstRect:actualRange:) 

Instance Method

# view(for:firstRect:actualRange:)

macOS

``` source
func view(
    for range: NSRange,
    firstRect: NSRectPointer?,
    actualRange: NSRangePointer?
) -> NSView?
```

**Required**

## See Also

### Instance Methods

func addAnnotations([NSAttributedString.Key : String], range: NSRange)

**Required**

func annotatedSubstring(forProposedRange: NSRange, actualRange: NSRangePointer?) -> NSAttributedString?

**Required**

func candidateListTouchBarItem() -> NSCandidateListTouchBarItem&lt;AnyObject>?

**Required**

func removeAnnotation(NSAttributedString.Key, range: NSRange)

**Required**

func replaceCharacters(in: NSRange, withAnnotatedString: NSAttributedString)

**Required**

func selectAndShow(NSRange)

**Required**

func setAnnotations([NSAttributedString.Key : String], range: NSRange)

**Required**

