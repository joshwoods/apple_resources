

- AppKit
-  NSTextCheckingClient 

Protocol

# NSTextCheckingClient

macOS

``` source
protocol NSTextCheckingClient : NSTextInputClient, NSTextInputTraits
```

## Topics

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

func view(for: NSRange, firstRect: NSRectPointer?, actualRange: NSRangePointer?) -> NSView?

**Required**

## Relationships

### Inherits From

- NSTextInputClient
- NSTextInputTraits

## See Also

### Text-checking

class NSTextCheckingController

protocol NSTextInputTraits

enum NSTextInputTraitType

