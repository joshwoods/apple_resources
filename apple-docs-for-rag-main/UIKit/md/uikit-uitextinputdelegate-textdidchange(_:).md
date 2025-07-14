

- UIKit
- UITextInputDelegate
-  textDidChange(\_:) 

Instance Method

# textDidChange(\_:)

Tells the input delegate when text has changed in the document.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func textDidChange(_ textInput: (any UITextInput)?)
```

**Required**

## Parameters 

`textInput`  

The document instance whose class adopts the UITextInput protocol.

## See Also

### Related Documentation

func selectionDidChange((any UITextInput)?)

Tells the input delegate when the selection has changed in the document.

**Required**

### Notifying the delegate of textual changes

func textWillChange((any UITextInput)?)

Tells the input delegate when text is about to change in the document.

**Required**

