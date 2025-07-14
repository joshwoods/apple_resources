

- UIKit
- UIPasteboard
-  isPersistent Deprecated

Instance Property

# isPersistent

A Boolean value that indicates whether the pasteboard is persistent.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var isPersistent: Bool { get }
```

Deprecated

Use shared app group containers instead. For more information about app groups, see Adding an App to an App Group. For more information about shared containers, see the containerURL(forSecurityApplicationGroupIdentifier:) method of FileManager (Swift) or the containerURLForSecurityApplicationGroupIdentifier: method of NSFileManager (Objective-C).

## Discussion

Nonpersistent named pasteboards remain available. You can use these to implement such features as Duplicate or Copy Style. A nonpersistent named pasteboard is available only in the process that creates it.

## See Also

### Related Documentation

init?(name: UIPasteboard.Name, create: Bool)

Returns a pasteboard that you identify by name, optionally creating it if it doesn’t exist.

class func withUniqueName() -> UIPasteboard

Returns an app pasteboard that you identify by a unique system-generated name.

### Deprecated

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

