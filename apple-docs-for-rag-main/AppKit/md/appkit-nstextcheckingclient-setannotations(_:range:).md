

- AppKit
- NSTextCheckingClient
-  setAnnotations(\_:range:) 

Instance Method

# setAnnotations(\_:range:)

macOS 10.0+

``` source
func setAnnotations(
    _ annotations: [NSAttributedString.Key : String],
    range: NSRange
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

func replaceCharacters(in: NSRange, withAnnotatedString: NSAttributedString)

**Required**

func selectAndShow(NSRange)

**Required**

func view(for: NSRange, firstRect: NSRectPointer?, actualRange: NSRangePointer?) -> NSView?

**Required**

