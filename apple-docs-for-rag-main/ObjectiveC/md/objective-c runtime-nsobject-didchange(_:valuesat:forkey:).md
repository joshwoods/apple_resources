

- Objective-C Runtime
- NSObject
-  didChange(\_:valuesAt:forKey:) 

Instance Method

# didChange(\_:valuesAt:forKey:)

Informs the observed object that the specified change has occurred on the indexes for a specified ordered to-many relationship.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func didChange(
    _ changeKind: NSKeyValueChange,
    valuesAt indexes: IndexSet,
    forKey key: String
)
```

## Parameters 

`changeKind`  

The type of change that was made.

`indexes`  

The indexes of the to-many relationship that were affected by the change.

`key`  

The name of a property that is an ordered to-many relationship.

## Discussion

Use this method when implementing key-value-observing compliance manually.

### Special Considerations

You rarely need to override this method in subclasses, but if you do, be sure to call `super`. Calls to this method are always paired with a matching call to willChange(_:valuesAt:forKey:).

## See Also

### Notifying Observers of Changes

func willChangeValue(forKey: String)

Informs the observed object that the value of a given property is about to change.

func didChangeValue(forKey: String)

Informs the observed object that the value of a given property has changed.

func willChange(NSKeyValueChange, valuesAt: IndexSet, forKey: String)

Informs the observed object that the specified change is about to be executed at given indexes for a specified ordered to-many relationship.

func willChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Informs the observed object that the specified change is about to be made to a specified unordered to-many relationship.

func didChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Informs the observed object that the specified change was made to a specified unordered to-many relationship.

