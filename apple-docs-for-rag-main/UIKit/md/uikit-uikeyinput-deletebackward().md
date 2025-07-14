

- UIKit
- UIKeyInput
-  deleteBackward() 

Instance Method

# deleteBackward()

Deletes a character from the displayed text.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func deleteBackward()
```

**Required**

## Mentioned in 

Handling text interactions in custom keyboards

## Discussion

Remove the character just before the cursor from your class’s backing store and redisplay the text.

## See Also

### Inserting and deleting text

func insertText(String)

Inserts a character into the displayed text.

**Required**

var hasText: Bool

A Boolean value that indicates whether the text-entry object has any text.

**Required**

