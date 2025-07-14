

- AppKit
- NSDocument
-  duplicate(\_:) 

Instance Method

# duplicate(\_:)

Creates a copy of the receiving document in response to the user choosing Duplicate from the File menu.

macOS 10.7+

``` source
@IBAction @MainActor
func duplicate(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the action message.

## Discussion

The default implementation of this method merely invokes `[self duplicateDocumentWithDelegate:nil didDuplicateSelector:NULL contextInfo:NULL]`.

## See Also

### Duplicating the Document

func duplicate() throws -> NSDocument

Creates a new document whose contents are the same as the receiver and returns an error object if unsuccessful.

func duplicate(withDelegate: Any?, didDuplicate: Selector?, contextInfo: UnsafeMutableRawPointer?)

Creates a new document whose contents are the same as the current document.

