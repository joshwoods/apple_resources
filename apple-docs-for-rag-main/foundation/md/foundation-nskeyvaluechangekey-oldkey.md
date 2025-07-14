

- Foundation
- NSKeyValueChangeKey
-  oldKey 

Type Property

# oldKey

If the value of the kindKey entry is NSKeyValueChange.setting, and old was specified when the observer was registered, the value of this key is the value before the attribute was changed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let oldKey: NSKeyValueChangeKey
```

## Discussion

For NSKeyValueChange.removal or NSKeyValueChange.replacement, if old was specified when the observer was registered, the value is an `NSArray` instance that contains the objects that have been removed or have been replaced by other objects, respectively.

## See Also

### Type Properties

static let indexesKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.insertion, NSKeyValueChange.removal, or NSKeyValueChange.replacement, the value of this key is an `NSIndexSet` object that contains the indexes of the inserted, removed, or replaced objects.

static let kindKey: NSKeyValueChangeKey

An `NSNumber` object that contains a value corresponding to one of the NSKeyValueChange enums, indicating what sort of change has occurred.

static let newKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.setting, and new was specified when the observer was registered, the value of this key is the new value for the attribute.

static let notificationIsPriorKey: NSKeyValueChangeKey

If the prior option was specified when the observer was registered this notification is sent prior to a change.

