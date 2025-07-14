

- Foundation
- NSAttributedString
-  containsAttachments(in:) 

Instance Method

# containsAttachments(in:)

Returns a Boolean value that indicates if the attributed string contains an attachment in the specified range.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func containsAttachments(in range: NSRange) -> Bool
```

## Parameters 

`range`  

The range.

## Return Value

true if the attributed string contains a property configured as attachment with character in `range`; otherwise, false.

## See Also

### Getting metrics for the string

func size() -> CGSize

Returns the size necessary to draw the string.

func boundingRect(with: CGSize, options: NSStringDrawingOptions, context: NSStringDrawingContext?) -> CGRect

Returns the bounding rectangle necessary to draw the string.

