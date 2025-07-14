

- Foundation
- NSAttributedString
-  containsAttachments Deprecated

Instance Property

# containsAttachments

A Boolean value that indicates whether the attribute string contains any attachment attributes.

macOS 10.0+

``` source
var containsAttachments: Bool { get }
```

Deprecated

Use containsAttachments(in:) instead.

## Return Value

YES if the attributed string contains any attachment attributes, otherwise NO.

## Discussion

This method checks only for attachment attributes, not for `NSAttachmentCharacter`.

