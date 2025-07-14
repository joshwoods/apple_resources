

- AppKit
- NSTextViewDelegate
-  textView(\_:willShow:forItems:) 

Instance Method

# textView(\_:willShow:forItems:)

Returns a sharing service picker for the current selection.

macOS 10.8+

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    willShow servicePicker: NSSharingServicePicker,
    forItems items: [Any]
) -> NSSharingServicePicker?
```

## Parameters 

`textView`  

The text view.

`servicePicker`  

The service picker.

`items`  

The ranges of the items to share.

## Return Value

An NSSharingServicePicker instance. The original sharing picker or a new sharing picker instance can be returned.

## Discussion

Returns a sharing service picker created for items right before shown to the screen when the `orderFrontSharingServicePicker:` method. Return `nil` to remove the Share item from the menu.

The delegate is specified as the delegate for the `NSSharingServicePicker` instance.

