

- UIKit
- UITextInputDelegate
-  selectionDidChange(\_:) 

Instance Method

# selectionDidChange(\_:)

Tells the input delegate when the selection has changed in the document.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func selectionDidChange(_ textInput: (any UITextInput)?)
```

**Required**

## Parameters 

`textInput`  

The document instance whose class adopts the UITextInput protocol.

## See Also

### Related Documentation

func textDidChange((any UITextInput)?)

Tells the input delegate when text has changed in the document.

**Required**

### Notifying the delegate of selection changes

func selectionWillChange((any UITextInput)?)

Tells the input delegate when the selection is about to change in the document.

**Required**

