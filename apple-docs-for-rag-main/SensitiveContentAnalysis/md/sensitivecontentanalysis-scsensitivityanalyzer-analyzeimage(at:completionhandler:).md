

- SensitiveContentAnalysis
- SCSensitivityAnalyzer
-  analyzeImage(at:completionHandler:) 

Instance Method

# analyzeImage(at:completionHandler:)

Analyzes an image file on disk at a URL and runs code on completion.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
func analyzeImage(
    at fileURL: URL,
    completionHandler: @escaping (SCSensitivityAnalysis?, (any Error)?) -> Void
)
```

``` source
func analyzeImage(at fileURL: URL) async throws -> SCSensitivityAnalysis
```

## Parameters 

`fileURL`  

The URL for an image file on disk.

`completionHandler`  

Code that your app provides for the system to run on completion.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func analyzeImage(at fileURL: URL) async throws -> SCSensitivityAnalysis
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The completion handler:

- Runs on an unspecified queue.

- Provides a `results` parameter that indicates if checked content contains nudity.

## See Also

### Analyzing images

func analyzeImage(CGImage, completionHandler: (SCSensitivityAnalysis?, (any Error)?) -> Void)

Analyzes an image for sensitive content and runs code on completion.

