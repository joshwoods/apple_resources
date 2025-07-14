

- AppKit
- NSTextCheckingClient
-  candidateListTouchBarItem() 

Instance Method

# candidateListTouchBarItem()

macOS 10.12.2+

``` source
func candidateListTouchBarItem() -> NSCandidateListTouchBarItem?
```

**Required**

## See Also

### Instance Methods

func addAnnotations([NSAttributedString.Key : String], range: NSRange)

**Required**

func annotatedSubstring(forProposedRange: NSRange, actualRange: NSRangePointer?) -> NSAttributedString?

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

