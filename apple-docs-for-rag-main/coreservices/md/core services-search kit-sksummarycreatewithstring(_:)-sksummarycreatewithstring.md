

- Core Services
- Search Kit
-  SKSummaryCreateWithString(\_:) 

Function

# SKSummaryCreateWithString(\_:)

Creates a summary object based on a text string.

macOS 10.4+

``` source
func SKSummaryCreateWithString(_ inString: CFString!) -> Unmanaged!
```

## Parameters 

`inString`  

The text string that you want to summarize.

## Return Value

Returns a summarization object, or `NULL` on failure.

## Discussion

The `SKSummaryCreateWithString(_:)` function creates a summarization object that pre-analyzes a text string to support fast summarization. When your application no longer needs the summarization object, dispose of it by calling CFRelease.

## See Also

### Working With Summarization

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

func SKSummaryGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit summarization objects.

