

- PDFKit
- PDFDocument
-  beginFindString(\_:withOptions:) 

Instance Method

# beginFindString(\_:withOptions:)

Asynchronously finds all instances of the specified string in the document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func beginFindString(
    _ string: String,
    withOptions options: NSString.CompareOptions = []
)
```

## Discussion

This method returns immediately. It causes notifications to be issued when searching begins and ends, on each search hit, and when the search proceeds to a new page. For options, refer to Searching, Comparing, and Sorting Strings.

## See Also

### Searching Documents

func findString(String, withOptions: NSString.CompareOptions) -> [PDFSelection]

Synchronously finds all instances of the specified string in the document.

func beginFindStrings([String], withOptions: NSString.CompareOptions)

Asynchronously finds all instances of the specified array of strings in the document.

func findString(String, fromSelection: PDFSelection?, withOptions: NSString.CompareOptions) -> PDFSelection?

Synchronously finds the next occurance of a string after the specified selection (or before the selection if you specified `NSBackwardsSearch` as a search option.

var isFinding: Bool

Returns a Boolean value indicating whether an asynchronous find operation is in progress.

func cancelFindString()

Cancels a search initiated with beginFindString(_:withOptions:).

