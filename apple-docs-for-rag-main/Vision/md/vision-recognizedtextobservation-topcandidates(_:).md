

- Vision
- RecognizedTextObservation
-  topCandidates(\_:) 

Instance Method

# topCandidates(\_:)

Requests the top candidates for a recognized text string.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func topCandidates(_ maxCandidateCount: Int) -> [RecognizedText]
```

## Parameters 

`maxCandidateCount`  

The maximum number of candidates to return, up to `10`.

## See Also

### Getting the recognized text

struct RecognizedText

Text recognized in an image through a text recognition request.

