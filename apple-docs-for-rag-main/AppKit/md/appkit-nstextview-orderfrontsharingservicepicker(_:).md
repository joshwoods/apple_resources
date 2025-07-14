

- AppKit
- NSTextView
-  orderFrontSharingServicePicker(\_:) 

Instance Method

# orderFrontSharingServicePicker(\_:)

Creates and displays a new instance of the sharing service picker.

macOS 10.8+

``` source
@IBAction @MainActor
func orderFrontSharingServicePicker(_ sender: Any?)
```

## Parameters 

`sender`  

The sender.

## Discussion

Creates a new instance of NSSharingServicePicker based on the current selection and shows to the screen. The items passed to the NSSharingServicePicker initializer are determined using the delegate method `textView:willShowSharingServicePicker:forItems:`.

When the current selection is 0 length, the whole document is passed to the method.

