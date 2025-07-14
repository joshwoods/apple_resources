

- UIKit
- UIKeyInput
-  hasText 

Instance Property

# hasText

A Boolean value that indicates whether the text-entry object has any text.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var hasText: Bool { get }
```

**Required**

## Return Value

true if the backing store has textual content, false otherwise.

## Mentioned in 

Handling text interactions in custom keyboards

## See Also

### Inserting and deleting text

func insertText(String)

Inserts a character into the displayed text.

**Required**

func deleteBackward()

Deletes a character from the displayed text.

**Required**

