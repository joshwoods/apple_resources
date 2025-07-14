

- Objective-C Runtime
- NSObject
-  willChangeValue(forKey:) 

Instance Method

# willChangeValue(forKey:)

Informs the observed object that the value of a given property is about to change.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func willChangeValue(forKey key: String)
```

## Parameters 

`key`  

The name of the property that will change.

## Discussion

Use this method when implementing key-value observer compliance manually to inform the observed object that the value at `key` is about to change.

The change type of this method is `NSKeyValueChangeSetting`.

Important

After the values have been changed, a corresponding didChangeValue(forKey:) must be invoked with the same parameter.

### Special Considerations

You rarely need to override this method in subclasses, but if you do, be sure to call `super`.

## See Also

### Notifying Observers of Changes

func didChangeValue(forKey: String)

Informs the observed object that the value of a given property has changed.

func willChange(NSKeyValueChange, valuesAt: IndexSet, forKey: String)

Informs the observed object that the specified change is about to be executed at given indexes for a specified ordered to-many relationship.

func didChange(NSKeyValueChange, valuesAt: IndexSet, forKey: String)

Informs the observed object that the specified change has occurred on the indexes for a specified ordered to-many relationship.

func willChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Informs the observed object that the specified change is about to be made to a specified unordered to-many relationship.

func didChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Informs the observed object that the specified change was made to a specified unordered to-many relationship.

