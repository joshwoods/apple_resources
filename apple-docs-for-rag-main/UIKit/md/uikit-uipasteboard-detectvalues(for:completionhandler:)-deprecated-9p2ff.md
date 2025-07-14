

- UIKit
- UIPasteboard
-  detectValues(for:completionHandler:) Deprecated

Instance Method

# detectValues(for:completionHandler:)

Determines whether the first pasteboard item matches the specified patterns, reading the contents if it finds a match.

iOS 14.0–15.0DeprecatediPadOS 14.0–15.0DeprecatedMac CatalystvisionOS 1.0–1.0Deprecated

``` source
func detectValues(
    for patterns: Set,
    completionHandler: @escaping (Result) -> ()
)
```

Deprecated

Use detectValues(for:completionHandler:) instead.

## Parameters 

`patterns`  

The patterns to detect on the pasteboard.

`completionHandler`  

A closure that the system invokes after detecting patterns on the pasteboard. The closure receives a `Result` instance that contains either a dictionary with the patterns found on the pasteboard or an error if detection failed. If the `Result` instance contains a dictionary, the keys specify the matched pattern, and the value specifies the content of the pasteboard.

## Discussion

Important

Calling this method notifies the user that the app has read the contents of the pasteboard.

For details about the types returned for each pattern, see UIPasteboard.DetectionPattern.

## See Also

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

func detectValues(for: Set&lt;UIPasteboard.DetectionPattern>, inItemSet: IndexSet?, completionHandler: (Result&lt;[[UIPasteboard.DetectionPattern : Any]], any Error>) -> ())

Determines whether pasteboard items match the specified patterns, reading the contents if it finds a match.

Deprecated

