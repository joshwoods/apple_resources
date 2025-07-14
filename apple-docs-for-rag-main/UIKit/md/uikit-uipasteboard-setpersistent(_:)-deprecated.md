

- UIKit
- UIPasteboard
-  setPersistent(\_:) Deprecated

Instance Method

# setPersistent(\_:)

A Boolean value that indicates whether the pasteboard is persistent.

iOS 3.0–10.0DeprecatediPadOS 3.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func setPersistent(_ persistent: Bool)
```

Deprecated

Use shared app group containers instead. For more information about app groups, see Adding an App to an App Group. For more information about shared containers, see the containerURL(forSecurityApplicationGroupIdentifier:) method of FileManager.

## Discussion

Nonpersistent named pasteboards remain available. You can use these to implement such features as Duplicate or Copy Style. A nonpersistent named pasteboard is available only in the process that creates it.

## See Also

### Deprecated

var isPersistent: Bool

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

