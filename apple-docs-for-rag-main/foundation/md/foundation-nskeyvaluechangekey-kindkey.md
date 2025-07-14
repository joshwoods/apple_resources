

- Foundation
- NSKeyValueChangeKey
-  kindKey 

Type Property

# kindKey

An `NSNumber` object that contains a value corresponding to one of the NSKeyValueChange enums, indicating what sort of change has occurred.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let kindKey: NSKeyValueChangeKey
```

## Discussion

A value of NSKeyValueChange.setting indicates that the observed object has received a setValue(_:forKey:) message, or that the key-value-coding-compliant set method for the key has been invoked, or that one of the willChangeValue(forKey:) or didChangeValue(forKey:) methods has otherwise been invoked.

A value of NSKeyValueChange.insertion, NSKeyValueChange.removal, or NSKeyValueChange.replacement indicates that mutating messages have been sent a key-value observing compliant collection proxy, or that one of the key-value-coding-compliant collection mutation methods for the key has been invoked, or a collection will change or did change method has been otherwise been invoked.

You can use the uintValue method on the `NSNumber` object to retrieve the value of the change kind.

## See Also

### Type Properties

static let indexesKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.insertion, NSKeyValueChange.removal, or NSKeyValueChange.replacement, the value of this key is an `NSIndexSet` object that contains the indexes of the inserted, removed, or replaced objects.

static let newKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.setting, and new was specified when the observer was registered, the value of this key is the new value for the attribute.

static let notificationIsPriorKey: NSKeyValueChangeKey

If the prior option was specified when the observer was registered this notification is sent prior to a change.

static let oldKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.setting, and old was specified when the observer was registered, the value of this key is the value before the attribute was changed.

