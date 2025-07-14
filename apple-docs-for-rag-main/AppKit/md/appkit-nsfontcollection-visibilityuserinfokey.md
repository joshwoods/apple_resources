

- AppKit
- NSFontCollection
-  visibilityUserInfoKey 

Type Property

# visibilityUserInfoKey

The visibly of the font collection. An NSNumber containing a value from the NSFontCollection.Visibility enum.

macOS 10.7+

``` source
class let visibilityUserInfoKey: NSFontCollection.UserInfoKey
```

## See Also

### User Info Keys

class let actionUserInfoKey: NSFontCollection.UserInfoKey

An action was taken. See `NSFontCollectionAction Key Values` for the possible values. An `NSString`.

class let nameUserInfoKey: NSFontCollection.UserInfoKey

The font collection’s name. If renamed, this is the new name. An `NSString`.

class let oldNameUserInfoKey: NSFontCollection.UserInfoKey

Included as a value for the oldNameUserInfoKey key, if present. This is the previous name. An `NSString`.

