

- Core Services
- Search Kit
-  SKSummaryCopySentenceAtIndex(\_:\_:) 

Function

# SKSummaryCopySentenceAtIndex(\_:\_:)

Gets a specified sentence from the text in a summarization object.

macOS 10.4+

``` source
func SKSummaryCopySentenceAtIndex(
    _ summary: SKSummary!,
    _ i: CFIndex
) -> Unmanaged!
```

## Parameters 

`summary`  

The summarization object containing the text from which you want a sentence.

`i`  

The ordinal number of the sentence in the original text, with the first sentence designated by zero (this function uses zero-based indexing).

## Return Value

A `CFString` object containing the specified sentence, or `NULL` on failure.

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

func SKSummaryCopyParagraphAtIndex(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a specified paragraph from the text in a summarization object.

func SKSummaryCopySentenceSummaryString(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a text string consisting of a summary with, at most, the requested number of sentences.

func SKSummaryCopyParagraphSummaryString(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a text string consisting of a summary with, at most, the requested number of paragraphs.

func SKSummaryGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit summarization objects.

