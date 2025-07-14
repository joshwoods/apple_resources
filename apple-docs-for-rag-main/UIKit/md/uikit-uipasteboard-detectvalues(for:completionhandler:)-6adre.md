

- UIKit
- UIPasteboard
-  detectValues(for:completionHandler:) 

Instance Method

# detectValues(for:completionHandler:)

Requests that the data detection system identify the types of data that you specify for the pasteboard, and provide the values that it matches to your closure.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
func detectValues(
    for keyPaths: Set>,
    completionHandler: @escaping (Result) -> ()
)
```

## Parameters 

`keyPaths`  

A set of key paths you use to indicate which types of data you want the data detection system to match.

`completionHandler`  

A closure you provide to process data the data detection system matches, or to handle errors.

## Discussion

Because this method gives the app access to the values it detects in the pasteboard, the system notifies the user about reading the contents of the pasteboard.

## See Also

### Detecting patterns of content in pasteboard items

func detectPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, completionHandler: (Result&lt;Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, any Error>) -> ())

Requests that the data detection system identify the patterns that you specify for the pasteboard, and provide the patterns that it matches to your closure.

func detectedPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>) async throws -> Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>

Requests that the data detection system asynchronously identify the patterns that you specify for the pasteboard, and return the patterns that it matches.

func detectPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?, completionHandler: (Result&lt;[Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>], any Error>) -> ())

Requests that the data detection system identify the patterns that you specify for the pasteboard items, and provide the patterns that it matches to your closure.

func detectedPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?) async throws -> [Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>]

Requests that the data detection system asynchronously identify the patterns that you specify for the pasteboard items, and return the patterns that it matches.

func detectedValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>) async throws -> UIPasteboard.DetectedValues

Requests that the data detection system asynchronously identify the types of values that you specify for the pasteboard, and return the values that it matches.

func detectValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?, completionHandler: (Result&lt;[UIPasteboard.DetectedValues], any Error>) -> ())

Requests that the data detection system identify the types of data that you specify for the pasteboard items, and provide the values that it matches to your closure.

func detectedValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?) async throws -> [UIPasteboard.DetectedValues]

Requests that the data detection system asynchronously identify the types of values that you specify for the pasteboard item, and return the values that it matches for each pasteboard.

struct DetectedValues

An object that contains common types of data that the data detection system matches for a pasteboard.

struct DetectionPattern

An object that represents a pattern to detect for the pasteboard, such as a URL, text, or a number.

