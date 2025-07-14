

- UIKit
- UIPasteboard
-  detectPatterns(for:completionHandler:) Deprecated

Instance Method

# detectPatterns(for:completionHandler:)

Determines whether the first pasteboard item matches the specified patterns, without notifying the user.

iOS 14.0–15.0DeprecatediPadOS 14.0–15.0DeprecatedMac CatalystvisionOS 1.0–1.0Deprecated

``` source
func detectPatterns(
    for patterns: Set,
    completionHandler: @escaping (Result, any Error>) -> ()
)
```

Deprecated

Use detectPatterns(for:completionHandler:) instead.

## Parameters 

`patterns`  

The patterns to detect on the pasteboard.

`completionHandler`  

A closure that the system invokes after detecting patterns on the pasteboard. The closure receives a `Result` instance that contains either a set with the patterns found on the pasteboard or an error if detection failed.

## Discussion

Because this method only gives an indication of whether a pasteboard item matches a particular pattern and doesn’t allow the app to access the contents, the system doesn’t notify the user about reading the contents of the pasteboard.

## See Also

### Deprecated

var isPersistent: Bool

A Boolean value that indicates whether the pasteboard is persistent.

Deprecated

func setPersistent(Bool)

A Boolean value that indicates whether the pasteboard is persistent.

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

