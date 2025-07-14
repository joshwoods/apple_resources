

- AppKit
- NSTextCheckingClient
-  replaceCharacters(in:withAnnotatedString:) 

Instance Method

# replaceCharacters(in:withAnnotatedString:)

macOS 10.0+

``` source
func replaceCharacters(
    in range: NSRange,
    withAnnotatedString annotatedString: NSAttributedString
)
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

func selectAndShow(NSRange)

**Required**

func setAnnotations([NSAttributedString.Key : String], range: NSRange)

**Required**

func view(for: NSRange, firstRect: NSRectPointer?, actualRange: NSRangePointer?) -> NSView?

**Required**

