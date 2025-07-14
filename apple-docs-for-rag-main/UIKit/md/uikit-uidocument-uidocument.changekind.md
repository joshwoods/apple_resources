

- UIKit
- UIDocument
-  UIDocument.ChangeKind 

Enumeration

# UIDocument.ChangeKind

Constants that specify the kind of change to a document.

iOSiPadOSMac CatalystvisionOS

``` source
enum ChangeKind
```

## Overview

You specify one of these constants as a parameter of the updateChangeCount(_:) method.

## Topics

### Constants

case done

A change has been made to the document.

case undone

A change to the document has been undone.

case redone

An undone change to the document has been redone.

case cleared

The document is cleared of outstanding changes.

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

enum SaveOperation

Constants that specify the type of save operation.

struct State

Constants that specify the document state.

class let userActivityURLKey: String

The key that identifies the document associated with a user activity.

