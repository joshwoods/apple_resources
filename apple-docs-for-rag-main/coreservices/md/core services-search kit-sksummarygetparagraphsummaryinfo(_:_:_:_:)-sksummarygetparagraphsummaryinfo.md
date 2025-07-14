

- Core Services
- Search Kit
-  SKSummaryGetParagraphSummaryInfo(\_:\_:\_:\_:) 

Function

# SKSummaryGetParagraphSummaryInfo(\_:\_:\_:\_:)

Gets detailed information about a body of text for constructing a custom paragraph-based summary string.

macOS 10.4+

``` source
func SKSummaryGetParagraphSummaryInfo(
    _ summary: SKSummary!,
    _ numParagraphsInSummary: CFIndex,
    _ outRankOrderOfParagraphs: UnsafeMutablePointer!,
    _ outParagraphIndexOfParagraphs: UnsafeMutablePointer!
) -> CFIndex
```

## Parameters 

`summary`  

The summarization object containing the text from which you want to build a summary.

`numParagraphsInSummary`  

The maximum number of paragraphs you want in the summary.

`outRankOrderOfParagraphs`  

On input, a pointer to an array of CFIndex objects. On output, points to the previously allocated array, which now lists the summarization relevance rank of each paragraph in the original text. The most important paragraph gets a rank of 1. The array size must equal `numParagraphsInSummary`, or else be `NULL` if you don’t want to get the relevance ranks.

`outParagraphIndexOfParagraphs`  

On output, points to an array containing the ordinal number for each paragraph in the original text. Use the SKSummaryCopyParagraphAtIndex(_:_:) function with one of these numbers to get the corresponding paragraph. The array size must equal `numParagraphsInSummary`, or else be `NULL` if you don’t want to get the ordinal numbers of the paragraphs.

## Return Value

The number of paragraphs in the summary.

## See Also

### Working With Summarization

func SKSummaryCreateWithString(CFString!) -> Unmanaged&lt;SKSummary>!

Creates a summary object based on a text string.

func SKSummaryGetSentenceSummaryInfo(SKSummary!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!) -> CFIndex

Gets detailed information about a body of text for constructing a custom sentence-based summary string.

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

func SKSummaryGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit summarization objects.

