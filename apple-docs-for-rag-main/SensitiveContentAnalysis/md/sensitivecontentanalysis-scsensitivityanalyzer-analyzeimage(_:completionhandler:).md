

- SensitiveContentAnalysis
- SCSensitivityAnalyzer
-  analyzeImage(\_:completionHandler:) 

Instance Method

# analyzeImage(\_:completionHandler:)

Analyzes an image for sensitive content and runs code on completion.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
func analyzeImage(
    _ image: CGImage,
    completionHandler: @escaping (SCSensitivityAnalysis?, (any Error)?) -> Void
)
```

``` source
func analyzeImage(_ image: CGImage) async throws -> SCSensitivityAnalysis
```

## Parameters 

`image`  

An image in memory.

`completionHandler`  

Code that your app provides for the system to run on completion.

## Mentioned in 

Testing your app’s response to sensitive media

## Discussion

The completion handler:

- Runs on an unspecified queue.

- Provides a `results` parameter that indicates if checked content contains nudity.

## See Also

### Analyzing images

func analyzeImage(at: URL, completionHandler: (SCSensitivityAnalysis?, (any Error)?) -> Void)

Analyzes an image file on disk at a URL and runs code on completion.

