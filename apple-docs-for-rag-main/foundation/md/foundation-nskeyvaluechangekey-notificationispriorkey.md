

- Foundation
- NSKeyValueChangeKey
-  notificationIsPriorKey 

Type Property

# notificationIsPriorKey

If the prior option was specified when the observer was registered this notification is sent prior to a change.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let notificationIsPriorKey: NSKeyValueChangeKey
```

## Discussion

The change dictionary contains an notificationIsPriorKey entry whose value is an `NSNumber` object that contains the Boolean value true.

## See Also

### Type Properties

static let indexesKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.insertion, NSKeyValueChange.removal, or NSKeyValueChange.replacement, the value of this key is an `NSIndexSet` object that contains the indexes of the inserted, removed, or replaced objects.

static let kindKey: NSKeyValueChangeKey

An `NSNumber` object that contains a value corresponding to one of the NSKeyValueChange enums, indicating what sort of change has occurred.

static let newKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.setting, and new was specified when the observer was registered, the value of this key is the new value for the attribute.

static let oldKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.setting, and old was specified when the observer was registered, the value of this key is the value before the attribute was changed.

