

- AVFoundation
- AVMutableCaption
-  setBackgroundColor(\_:in:) 

Instance Method

# setBackgroundColor(\_:in:)

Sets the background color for a range of text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func setBackgroundColor(
    _ backgroundColor: CGColor,
    in range: NSRange
)
```

## Parameters 

`backgroundColor`  

The background color.

`range`  

The range to which this background color applies.

## See Also

### Configuring Colors

func setTextColor(CGColor, in: NSRange)

Sets the text color for a range of text.

func removeTextColor(in: NSRange)

Removes the text color for a range of text.

func removeBackgroundColor(in: NSRange)

Removes a background color from a range of text.

