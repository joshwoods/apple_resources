

- UIKit
- UITextDocumentProxy
-  adjustTextPosition(byCharacterOffset:) 

Instance Method

# adjustTextPosition(byCharacterOffset:)

Moves the insertion point forward or backward in the current text input object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func adjustTextPosition(byCharacterOffset offset: Int)
```

**Required**

## Parameters 

`offset`  

The number of characters to adjust the insertion point by. A positive value moves the insertion point forward (according to the text storage direction for the current language). A negative value moves the insertion point backward.

## Mentioned in 

Handling text interactions in custom keyboards

