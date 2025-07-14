

- Collaboration
-  CBIdentityPicker 

Class

# CBIdentityPicker

A `CBIdentityPicker` object allows a user to select identities—for example, user or group objects—that it wants one or more services or shared resources to have access to. An identity picker can be displayed either as an application-modal dialog or as a sheet attached to a document window. An identity picker returns the selected records to be added to access control lists using Collaboration. If a selected record is not a user or group identity, then an identity picker prompts the user for additional information—such as a password—to promote that record to a sharing account.

macOS 10.5+

``` source
class CBIdentityPicker
```

## Topics

### Running an Identity Picker

func runModal(for: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the receiver modally as a sheet attached to a specified window.

Deprecated

func runModal(for: NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Runs the identity picker modally as a sheet attached to a specified window.

func runModal() -> Int

Runs the receiver as an application-modal dialog.

### Retrieving Identities

var identities: [CBIdentity]

The array of identities (represented by `CBIdentity` objects) selected using the identity picker.

### Setting and Getting Properties

var title: String?

The title of the identity picker.

var allowsMultipleSelection: Bool

A Boolean value indicating whether the user is allowed to select multiple identities.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

