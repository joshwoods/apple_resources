

- UIKit
- UITextInputDelegate
-  selectionWillChange(\_:) 

Instance Method

# selectionWillChange(\_:)

Tells the input delegate when the selection is about to change in the document.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func selectionWillChange(_ textInput: (any UITextInput)?)
```

**Required**

## Parameters 

`textInput`  

The document instance whose class adopts the UITextInput protocol.

## See Also

### Related Documentation

func textWillChange((any UITextInput)?)

Tells the input delegate when text is about to change in the document.

**Required**

### Notifying the delegate of selection changes

func selectionDidChange((any UITextInput)?)

Tells the input delegate when the selection has changed in the document.

**Required**

