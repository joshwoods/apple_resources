

- UIKit
- Documents, data, and pasteboard
- UIPasteboard
-  UserInfo Dictionary Keys 

API Collection

# UserInfo Dictionary Keys

Use these keys to access the representation types of pasteboard items that you add to, or remove from, a pasteboard.

## Topics

### Constants

class let changedTypesAddedUserInfoKey: String

With the notification named changedNotification, use this key to access the added representation types. These types are stored as an array in the notification’s `userInfo` dictionary.

class let changedTypesRemovedUserInfoKey: String

With the notification named changedNotification, use this key to access the removed representation types. These types are stored as an array in the notification’s `userInfo` dictionary.

## See Also

### Constants

struct Name

Constants that identify the name of a pasteboard.

Pasteboard Names

Names identifying the system pasteboards.

struct OptionsKey

Options for describing pasteboard privacy.

Pasteboard Data Type Representations

Pasteboard-item representation types, as for a given object value.

