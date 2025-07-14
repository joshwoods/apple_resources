

- UIKit
- UIDocument
-  UIDocument.SaveOperation 

Enumeration

# UIDocument.SaveOperation

Constants that specify the type of save operation.

iOSiPadOSMac CatalystvisionOS

``` source
enum SaveOperation
```

## Overview

You specify one of these constants as a parameter in the following methods: save(to:for:completionHandler:), writeContents(_:andAttributes:safelyTo:for:), writeContents(_:to:for:originalContentsURL:), fileAttributesToWrite(to:for:), fileNameExtension(forType:saveOperation:), changeCountToken(for:), and updateChangeCount(withToken:for:).

## Topics

### Constants

case forCreating

The document is being saved for the first time.

case forOverwriting

The document is being saved by overwriting the current version.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum ChangeKind

Constants that specify the kind of change to a document.

struct State

Constants that specify the document state.

class let userActivityURLKey: String

The key that identifies the document associated with a user activity.

