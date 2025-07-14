

- UIKit
- UIPasteboard
-  detectedPatterns(for:inItemSet:) 

Instance Method

# detectedPatterns(for:inItemSet:)

Requests that the data detection system asynchronously identify the patterns that you specify for the pasteboard items, and return the patterns that it matches.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
func detectedPatterns(
    for keyPaths: Set>,
    inItemSet itemSet: IndexSet?
) async throws -> [Set>]
```

## Parameters 

`keyPaths`  

A set of key paths you use to indicate which types of pattern you want the data detection system to match.

`itemSet`  

A set of indexes you provide to indicate which pasteboard items the data detection system inspects to detect patterns.

## Return Value

A set of key paths that represent the patterns the data detection system matches in the pasteboard.

## Discussion

Because this method only gives an indication of whether a pasteboard item matches a particular pattern and doesn’t allow the app to access the contents, the system doesn’t notify the user about reading the contents of the pasteboard.

## See Also

### Detecting patterns of content in pasteboard items

func detectPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, completionHandler: (Result&lt;Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, any Error>) -> ())

Requests that the data detection system identify the patterns that you specify for the pasteboard, and provide the patterns that it matches to your closure.

func detectedPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>) async throws -> Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>

Requests that the data detection system asynchronously identify the patterns that you specify for the pasteboard, and return the patterns that it matches.

func detectPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?, completionHandler: (Result&lt;[Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>], any Error>) -> ())

Requests that the data detection system identify the patterns that you specify for the pasteboard items, and provide the patterns that it matches to your closure.

func detectValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, completionHandler: (Result&lt;UIPasteboard.DetectedValues, any Error>) -> ())

Requests that the data detection system identify the types of data that you specify for the pasteboard, and provide the values that it matches to your closure.

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

