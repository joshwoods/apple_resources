

- Core Services
- Search Kit
-  SKSummaryGetSentenceSummaryInfo(\_:\_:\_:\_:\_:) 

Function

# SKSummaryGetSentenceSummaryInfo(\_:\_:\_:\_:\_:)

Gets detailed information about a body of text for constructing a custom sentence-based summary string.

macOS 10.4+

``` source
func SKSummaryGetSentenceSummaryInfo(
    _ summary: SKSummary!,
    _ numSentencesInSummary: CFIndex,
    _ outRankOrderOfSentences: UnsafeMutablePointer!,
    _ outSentenceIndexOfSentences: UnsafeMutablePointer!,
    _ outParagraphIndexOfSentences: UnsafeMutablePointer!
) -> CFIndex
```

## Parameters 

`summary`  

The summarization object containing the text from which you want to build a summary.

`numSentencesInSummary`  

The maximum number of sentences you want in the summary.

`outRankOrderOfSentences`  

On input, a pointer to an array of CFIndex objects. On output, points to the previously allocated array, which now lists the summarization relevance rank of each sentence in the original text. The most important sentence gets a rank of 1. The array size must equal `numSentencesInSummary`, or else be `NULL` if you don’t want to get the rank orders.

`outSentenceIndexOfSentences`  

On input, a pointer to an array of CFIndex objects. On output, points to the previously allocated array, which now contains the ordinal number for each sentence in the original text. Use the SKSummaryCopySentenceAtIndex(_:_:) function with one of these numbers to get the corresponding sentence. The array size must equal `numSentencesInSummary`, or else be `NULL` if you don’t want to get the ordinal numbers of the sentences.

`outParagraphIndexOfSentences`  

On input, a pointer to an array of CFIndex objects. On output, points to the previously allocated array, which now contains the ordinal number for the paragraph that each corresponding sentence, referenced in `outSentenceIndexOfSentences`, appears in. The array size must equal `numSentencesInSummary`, or else be `NULL` if you don’t want to get the ordinal numbers of the sentences.

## Return Value

The number of sentences in the summary.

## See Also

### Working With Summarization

func SKSummaryCreateWithString(CFString!) -> Unmanaged&lt;SKSummary>!

Creates a summary object based on a text string.

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

func SKSummaryGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit summarization objects.

