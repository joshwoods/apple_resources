

- File Provider
- Nonreplicated File Provider extension
- Content and Change Tracking
- Tracking Your File Provider’s Changes
-  Tracking Changes to Documents 

Article

# Tracking Changes to Documents

Track and report changes to open documents.

## Overview

The File Provider extension must report any changes to a document’s content while the user is viewing the document.

When an app opens a document managed by your File Provider extension (using either an NSFilePresenter or UIDocument object), the system requests an enumerator for that document. This enumerator is used only for tracking changes to the document from other processes (for example, updates from another device).

The document enumerator remains active as long as the document is open. Any calls to its enumerateChanges(for:from:) method should return only information about the specified document.

These changes are forwarded to the NSFilePresenter or UIDocument that is monitoring the document. The app then updates its user interface as needed.

