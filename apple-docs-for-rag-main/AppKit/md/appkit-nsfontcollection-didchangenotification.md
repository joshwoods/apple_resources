

- AppKit
- NSFontCollection
-  didChangeNotification 

Type Property

# didChangeNotification

Posted whenever a font collection is changed.

macOS 10.7+

``` source
class let didChangeNotification: NSNotification.Name
```

## Discussion

The notification’s object is the font collection that was affected. The notification’s `userInfo` dictionary contains information about the the collection change containing the keys defined in NSFontCollection.UserInfoKey and the corresponding values.

## See Also

### Responding to Changes

struct UserInfoKey

These constants are used as keys in the didChangeNotification `userInfo` dictionary to indicate the changes that have taken place.

struct ActionTypeKey

The following actions are possible values of the actionUserInfoKey in the didChangeNotification `userInfo` method.

