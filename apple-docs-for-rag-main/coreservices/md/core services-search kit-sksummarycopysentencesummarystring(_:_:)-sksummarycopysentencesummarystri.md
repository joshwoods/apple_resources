

- Core Services
- Search Kit
-  SKSummaryCopySentenceSummaryString(\_:\_:) 

Function

# SKSummaryCopySentenceSummaryString(\_:\_:)

Gets a text string consisting of a summary with, at most, the requested number of sentences.

macOS 10.4+

``` source
func SKSummaryCopySentenceSummaryString(
    _ summary: SKSummary!,
    _ numSentences: CFIndex
) -> Unmanaged!
```

## Parameters 

`summary`  

The summarization object containing the text from which you want a summarization.

`numSentences`  

The maximum number of sentences you want in the summary.

## Return Value

A `CFString` object containing the requested summary.

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

func SKSummaryCopyParagraphSummaryString(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a text string consisting of a summary with, at most, the requested number of paragraphs.

func SKSummaryGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit summarization objects.

