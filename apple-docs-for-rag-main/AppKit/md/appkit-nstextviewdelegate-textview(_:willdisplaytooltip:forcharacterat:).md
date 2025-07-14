

- AppKit
- NSTextViewDelegate
-  textView(\_:willDisplayToolTip:forCharacterAt:) 

Instance Method

# textView(\_:willDisplayToolTip:forCharacterAt:)

Returns the actual tooltip to display.

macOS

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    willDisplayToolTip tooltip: String,
    forCharacterAt characterIndex: Int
) -> String?
```

## Parameters 

`textView`  

The text view sending the message.

`tooltip`  

The proposed tooltip to display.

`characterIndex`  

The location in `textView`.

## Return Value

The actual tooltip to display, or `nil` to suppress display of the tooltip.

## Discussion

The tooltip string is the value of the toolTip attribute at `characterIndex`.

