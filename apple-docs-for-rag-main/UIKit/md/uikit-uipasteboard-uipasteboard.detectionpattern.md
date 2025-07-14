

- UIKit
- UIPasteboard
-  UIPasteboard.DetectionPattern 

Structure

# UIPasteboard.DetectionPattern

An object that represents a pattern to detect for the pasteboard, such as a URL, text, or a number.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
struct DetectionPattern
```

## Topics

### Detecting common patterns

static let number: UIPasteboard.DetectionPattern

A pattern that indicates the pasteboard contains a string that consists of a numeric value.

static let probableWebSearch: UIPasteboard.DetectionPattern

A pattern that indicates the pasteboard contains a string suitable for use as a web search term.

static let probableWebURL: UIPasteboard.DetectionPattern

A pattern that indicates the pasteboard contains a string that consists of a URL.

### Creating a detection pattern

init(rawValue: String)

Creates a detection pattern to detect different types of content on the pasteboard.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

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

