

- UIKit
- UIKeyInput
-  insertText(\_:) 

Instance Method

# insertText(\_:)

Inserts a character into the displayed text.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func insertText(_ text: String)
```

**Required**

## Parameters 

`text`  

A string object representing the character typed on the system keyboard.

## Mentioned in 

Handling text interactions in custom keyboards

## Discussion

Add the character `text` to your class’s backing store at the index corresponding to the cursor and redisplay the text.

## See Also

### Inserting and deleting text

func deleteBackward()

Deletes a character from the displayed text.

**Required**

var hasText: Bool

A Boolean value that indicates whether the text-entry object has any text.

**Required**

