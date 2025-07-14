

- UIKit
- UITextInputDelegate
-  textWillChange(\_:) 

Instance Method

# textWillChange(\_:)

Tells the input delegate when text is about to change in the document.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func textWillChange(_ textInput: (any UITextInput)?)
```

**Required**

## Parameters 

`textInput`  

The document instance whose class adopts the UITextInput protocol.

## Mentioned in 

Configuring a custom keyboard interface

## See Also

### Related Documentation

func selectionWillChange((any UITextInput)?)

Tells the input delegate when the selection is about to change in the document.

**Required**

### Notifying the delegate of textual changes

func textDidChange((any UITextInput)?)

Tells the input delegate when text has changed in the document.

**Required**

