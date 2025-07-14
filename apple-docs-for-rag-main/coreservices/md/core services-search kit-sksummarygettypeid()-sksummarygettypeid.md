

- Core Services
- Search Kit
-  SKSummaryGetTypeID() 

Function

# SKSummaryGetTypeID()

Gets the type identifier for Search Kit summarization objects.

macOS 10.4+

``` source
func SKSummaryGetTypeID() -> CFTypeID
```

## Return Value

A CFTypeID object, or `NULL` on failure.

## Discussion

Search Kit represents summarization results with summarization objects (SKSummary opaque types). If your code needs to determine whether a particular data type is a summary, you can use this function along with the CFGetTypeID(_:) function and perform a comparison.

Never hard-code the summarization type ID because it can change from one release of macOS to another.

## See Also

### Working With Summarization

func SKSummaryCreateWithString(CFString!) -> Unmanaged&lt;SKSummary>!

Creates a summary object based on a text string.

func SKSummaryGetSentenceSummaryInfo(SKSummary!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!) -> CFIndex

Gets detailed information about a body of text for constructing a custom sentence-based summary string.

func SKSummaryGetParagraphSummaryInfo(SKSummary!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!) -> CFIndex

Gets detailed information about a body of text for constructing a custom paragraph-based summary string.

func SKSummaryGetSentenceCount(SKSummary!) -> CFIndex

Gets the number of sentences in a summarization object.

func SKSummaryGetParagraphCount(SKSummary!) -> CFIndex

Gets the number of paragraphs in a summarization object.

func SKSummaryCopySentenceAtIndex(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a specified sentence from the text in a summarization object.

func SKSummaryCopyParagraphAtIndex(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a specified paragraph from the text in a summarization object.

func SKSummaryCopySentenceSummaryString(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a text string consisting of a summary with, at most, the requested number of sentences.

func SKSummaryCopyParagraphSummaryString(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a text string consisting of a summary with, at most, the requested number of paragraphs.

