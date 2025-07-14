

- AppKit
- NSDocument
- NSDocument.SaveOperationType
-  NSDocument.SaveOperationType.saveToOperation 

Case

# NSDocument.SaveOperationType.saveToOperation

An operation that writes a copy of the document’s contents to the specified location, without changing the original document’s location.

macOS

``` source
case saveToOperation
```

## See Also

### Constants

case saveOperation

An operation that overwrites a document’s file or file package with the document’s contents.

case saveAsOperation

An operation that writes the document’s contents to a new location and updates the document to point to that location

case autosaveElsewhereOperation

An operation that writes an autosave version of the file to a different location.

case autosaveInPlaceOperation

An operation that overwrites the document’s current contents with autosave data.

case autosaveAsOperation

An operation that writes a document’s contents to a new file or file package even though the user has not explicitly requested it, then changes the document’s current location to point to the just-written file or file package.

