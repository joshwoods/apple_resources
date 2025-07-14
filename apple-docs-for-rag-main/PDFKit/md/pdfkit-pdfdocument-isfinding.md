

- PDFKit
- PDFDocument
-  isFinding 

Instance Property

# isFinding

Returns a Boolean value indicating whether an asynchronous find operation is in progress.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var isFinding: Bool { get }
```

## See Also

### Searching Documents

func findString(String, withOptions: NSString.CompareOptions) -> [PDFSelection]

Synchronously finds all instances of the specified string in the document.

func beginFindString(String, withOptions: NSString.CompareOptions)

Asynchronously finds all instances of the specified string in the document.

func beginFindStrings([String], withOptions: NSString.CompareOptions)

Asynchronously finds all instances of the specified array of strings in the document.

func findString(String, fromSelection: PDFSelection?, withOptions: NSString.CompareOptions) -> PDFSelection?

Synchronously finds the next occurance of a string after the specified selection (or before the selection if you specified `NSBackwardsSearch` as a search option.

func cancelFindString()

Cancels a search initiated with beginFindString(_:withOptions:).

