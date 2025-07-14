

- AppKit
- NSFontCollection
-  NSFontCollection.UserInfoKey 

Structure

# NSFontCollection.UserInfoKey

These constants are used as keys in the didChangeNotification `userInfo` dictionary to indicate the changes that have taken place.

macOS

``` source
struct UserInfoKey
```

## Topics

### User Info Keys

class let actionUserInfoKey: NSFontCollection.UserInfoKey

An action was taken. See `NSFontCollectionAction Key Values` for the possible values. An `NSString`.

class let nameUserInfoKey: NSFontCollection.UserInfoKey

The font collection’s name. If renamed, this is the new name. An `NSString`.

class let oldNameUserInfoKey: NSFontCollection.UserInfoKey

Included as a value for the oldNameUserInfoKey key, if present. This is the previous name. An `NSString`.

class let visibilityUserInfoKey: NSFontCollection.UserInfoKey

The visibly of the font collection. An NSNumber containing a value from the NSFontCollection.Visibility enum.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Responding to Changes

class let didChangeNotification: NSNotification.Name

Posted whenever a font collection is changed.

struct ActionTypeKey

The following actions are possible values of the actionUserInfoKey in the didChangeNotification `userInfo` method.

