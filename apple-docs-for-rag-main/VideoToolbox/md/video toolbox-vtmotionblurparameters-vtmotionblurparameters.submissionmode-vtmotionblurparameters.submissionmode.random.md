

- Video Toolbox
- VTMotionBlurParameters
- VTMotionBlurParameters.SubmissionMode
-  VTMotionBlurParameters.SubmissionMode.random 

Case

# VTMotionBlurParameters.SubmissionMode.random

A submission follow presentation time order with a jump or skip in a frame sequence.

macOS 15.4+

``` source
case random
```

## Discussion

If this value is set, the internal cache will be cleared during the processWithParameters call.

## See Also

### Submission modes

case sequential

A submission follow presentation time order without a jump or skip when compared to a previous submission.

