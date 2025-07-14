

- UIKit
- Documents, data, and pasteboard
- UIPasteboard
-  Deprecated symbols 

API Collection

# Deprecated symbols

Review unsupported symbols and their replacements.

## Topics

### Deprecated

var isPersistent: Bool

A Boolean value that indicates whether the pasteboard is persistent.

Deprecated

func setPersistent(Bool)

A Boolean value that indicates whether the pasteboard is persistent.

Deprecated

func detectPatterns(for: Set&lt;UIPasteboard.DetectionPattern>, completionHandler: (Result&lt;Set&lt;UIPasteboard.DetectionPattern>, any Error>) -> ())

Determines whether the first pasteboard item matches the specified patterns, without notifying the user.

Deprecated

func detectPatterns(for: Set&lt;UIPasteboard.DetectionPattern>, inItemSet: IndexSet?, completionHandler: (Result&lt;[Set&lt;UIPasteboard.DetectionPattern>], any Error>) -> ())

Determines whether pasteboard items match the specified patterns, without notifying the user.

Deprecated

func detectValues(for: Set&lt;UIPasteboard.DetectionPattern>, completionHandler: (Result&lt;[UIPasteboard.DetectionPattern : Any], any Error>) -> ())

Determines whether the first pasteboard item matches the specified patterns, reading the contents if it finds a match.

Deprecated

func detectValues(for: Set&lt;UIPasteboard.DetectionPattern>, inItemSet: IndexSet?, completionHandler: (Result&lt;[[UIPasteboard.DetectionPattern : Any]], any Error>) -> ())

Determines whether pasteboard items match the specified patterns, reading the contents if it finds a match.

Deprecated

