

- UIKit
- UIPasteboard
-  detectPatterns(for:inItemSet:completionHandler:) Deprecated

Instance Method

# detectPatterns(for:inItemSet:completionHandler:)

Determines whether pasteboard items match the specified patterns, without notifying the user.

iOS 14.0–15.0DeprecatediPadOS 14.0–15.0DeprecatedMac CatalystvisionOS 1.0–1.0Deprecated

``` source
func detectPatterns(
    for patterns: Set,
    inItemSet itemSet: IndexSet?,
    completionHandler: @escaping (Result], any Error>) -> ()
)
```

Deprecated

Use detectPatterns(for:inItemSet:completionHandler:) instead.

## Parameters 

`patterns`  

The patterns to detect on the pasteboard.

`itemSet`  

An index set with each integer value identifying a pasteboard item positionally in the pasteboard. Pass `nil` to detect patterns in all pasteboard items.

`completionHandler`  

A closure that the system invokes after detecting patterns on the pasteboard. The closure receives a `Result` instance that contains either an array with the patterns found on the pasteboard or an error if detection failed. If the `Result` instance contains an array, the index of each element in the array corresponds to the pasteboard item index specified in `itemSet`.

## Discussion

Because this method only detects for the presence of patterns and does not read the contents of the pasteboard, the system doesn’t notify the user about reading the contents of the pasteboard.

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

func detectValues(for: Set&lt;UIPasteboard.DetectionPattern>, completionHandler: (Result&lt;[UIPasteboard.DetectionPattern : Any], any Error>) -> ())

Determines whether the first pasteboard item matches the specified patterns, reading the contents if it finds a match.

Deprecated

func detectValues(for: Set&lt;UIPasteboard.DetectionPattern>, inItemSet: IndexSet?, completionHandler: (Result&lt;[[UIPasteboard.DetectionPattern : Any]], any Error>) -> ())

Determines whether pasteboard items match the specified patterns, reading the contents if it finds a match.

Deprecated

