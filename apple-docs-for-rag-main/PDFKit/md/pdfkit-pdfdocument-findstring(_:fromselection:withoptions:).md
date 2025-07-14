

- PDFKit
- PDFDocument
-  findString(\_:fromSelection:withOptions:) 

Instance Method

# findString(\_:fromSelection:withOptions:)

Synchronously finds the next occurance of a string after the specified selection (or before the selection if you specified `NSBackwardsSearch` as a search option.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func findString(
    _ string: String,
    fromSelection selection: PDFSelection?,
    withOptions options: NSString.CompareOptions = []
) -> PDFSelection?
```

## Discussion

Matches are returned as a PDFSelection object. If the search reaches the end (or beginning) of the document without any hits, this method returns `NULL`.

If you pass `NULL` for the selection, this method begins searching from the beginning of the document (or the end, if you specified `NSBackwardsSearch`).

You can use this method to implement “Find Again” behavior. For options, refer to Searching, Comparing, and Sorting Strings.

## See Also

### Searching Documents

func findString(String, withOptions: NSString.CompareOptions) -> [PDFSelection]

Synchronously finds all instances of the specified string in the document.

func beginFindString(String, withOptions: NSString.CompareOptions)

Asynchronously finds all instances of the specified string in the document.

func beginFindStrings([String], withOptions: NSString.CompareOptions)

Asynchronously finds all instances of the specified array of strings in the document.

var isFinding: Bool

Returns a Boolean value indicating whether an asynchronous find operation is in progress.

func cancelFindString()

Cancels a search initiated with beginFindString(_:withOptions:).

