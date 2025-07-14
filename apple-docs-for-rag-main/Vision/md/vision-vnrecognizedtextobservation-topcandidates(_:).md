

- Vision
- VNRecognizedTextObservation
-  topCandidates(\_:) 

Instance Method

# topCandidates(\_:)

Requests the *n* top candidates for a recognized text string.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func topCandidates(_ maxCandidateCount: Int) -> [VNRecognizedText]
```

## Parameters 

`maxCandidateCount`  

The maximum number of candidates to return. This can’t exceed 10.

## Return Value

An array of the *n* top candidates, sorted by decreasing confidence score.

## Discussion

This function returns no more than *n* candidates, but it may return fewer than *n* candidates.

## See Also

### Obtaining Recognized Text

class VNRecognizedText

Text recognized in an image through a text recognition request.

