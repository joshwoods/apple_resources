

- Objective-C Runtime
- NSObject
-  didChangeValue(forKey:) 

Instance Method

# didChangeValue(forKey:)

Informs the observed object that the value of a given property has changed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func didChangeValue(forKey key: String)
```

## Parameters 

`key`  

The name of the property that changed.

## Discussion

Use this method when implementing key-value observer compliance manually to inform the observed object that the value at `key` has just changed. Calls to this method are always paired with a matching call to willChangeValue(forKey:).

### Special Considerations

You rarely need to override this method in subclasses, but if you do, be sure to call `super`.

## See Also

### Notifying Observers of Changes

func willChangeValue(forKey: String)

Informs the observed object that the value of a given property is about to change.

func willChange(NSKeyValueChange, valuesAt: IndexSet, forKey: String)

Informs the observed object that the specified change is about to be executed at given indexes for a specified ordered to-many relationship.

func didChange(NSKeyValueChange, valuesAt: IndexSet, forKey: String)

Informs the observed object that the specified change has occurred on the indexes for a specified ordered to-many relationship.

func willChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Informs the observed object that the specified change is about to be made to a specified unordered to-many relationship.

func didChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Informs the observed object that the specified change was made to a specified unordered to-many relationship.

