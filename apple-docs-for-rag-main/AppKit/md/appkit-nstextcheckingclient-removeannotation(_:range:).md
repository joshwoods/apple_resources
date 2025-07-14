

- AppKit
- NSTextCheckingClient
-  removeAnnotation(\_:range:) 

Instance Method

# removeAnnotation(\_:range:)

macOS 10.0+

``` source
func removeAnnotation(
    _ annotationName: NSAttributedString.Key,
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

func replaceCharacters(in: NSRange, withAnnotatedString: NSAttributedString)

**Required**

func selectAndShow(NSRange)

**Required**

func setAnnotations([NSAttributedString.Key : String], range: NSRange)

**Required**

func view(for: NSRange, firstRect: NSRectPointer?, actualRange: NSRangePointer?) -> NSView?

**Required**

