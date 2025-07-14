

- PDFKit
- PDFDocument
-  findString(\_:withOptions:) 

Instance Method

# findString(\_:withOptions:)

Synchronously finds all instances of the specified string in the document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func findString(
    _ string: String,
    withOptions options: NSString.CompareOptions = []
) -> [PDFSelection]
```

## Discussion

Each hit gets added to an `NSArray` object as a PDFSelection object. If there are no hits, this method returns an empty array.

Use this method when the complete search process will be brief and when you don’t need the flexibility or control offered by beginFindString(_:withOptions:). For options, refer to Searching, Comparing, and Sorting Strings.

## See Also

### Searching Documents

func beginFindString(String, withOptions: NSString.CompareOptions)

Asynchronously finds all instances of the specified string in the document.

func beginFindStrings([String], withOptions: NSString.CompareOptions)

Asynchronously finds all instances of the specified array of strings in the document.

func findString(String, fromSelection: PDFSelection?, withOptions: NSString.CompareOptions) -> PDFSelection?

Synchronously finds the next occurance of a string after the specified selection (or before the selection if you specified `NSBackwardsSearch` as a search option.

var isFinding: Bool

Returns a Boolean value indicating whether an asynchronous find operation is in progress.

func cancelFindString()

Cancels a search initiated with beginFindString(_:withOptions:).

