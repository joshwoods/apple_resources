

- AppKit
- NSTextCheckingClient
-  annotatedSubstring(forProposedRange:actualRange:) 

Instance Method

# annotatedSubstring(forProposedRange:actualRange:)

macOS 10.0+

``` source
func annotatedSubstring(
    forProposedRange range: NSRange,
    actualRange: NSRangePointer?
) -> NSAttributedString?
```

**Required**

## See Also

### Instance Methods

func addAnnotations([NSAttributedString.Key : String], range: NSRange)

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

func view(for: NSRange, firstRect: NSRectPointer?, actualRange: NSRangePointer?) -> NSView?

**Required**

