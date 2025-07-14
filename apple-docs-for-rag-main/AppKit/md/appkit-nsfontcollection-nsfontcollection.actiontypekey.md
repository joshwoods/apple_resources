

- AppKit
- NSFontCollection
-  NSFontCollection.ActionTypeKey 

Structure

# NSFontCollection.ActionTypeKey

The following actions are possible values of the actionUserInfoKey in the didChangeNotification `userInfo` method.

macOS

``` source
struct ActionTypeKey
```

## Topics

### Action Key Types

static let shown: NSFontCollection.ActionTypeKey

The font collection was shown.

static let hidden: NSFontCollection.ActionTypeKey

The font collection was hidden.

static let renamed: NSFontCollection.ActionTypeKey

The font collection was renamed.

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

struct UserInfoKey

These constants are used as keys in the didChangeNotification `userInfo` dictionary to indicate the changes that have taken place.

