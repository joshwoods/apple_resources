

- Objective-C Runtime
- NSObject
-  didChangeValue(forKey:withSetMutation:using:) 

Instance Method

# didChangeValue(forKey:withSetMutation:using:)

Informs the observed object that the specified change was made to a specified unordered to-many relationship.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func didChangeValue(
    forKey key: String,
    withSetMutation mutationKind: NSKeyValueSetMutationKind,
    using objects: Set
)
```

## Parameters 

`key`  

The name of a property that is an unordered to-many relationship

`mutationKind`  

The type of change that was made.

`objects`  

The objects that were involved in the change (see NSKeyValueSetMutationKind).

## Discussion

Use this method when implementing key-value observer compliance manually. Calls to this method are always paired with a matching call to willChangeValue(forKey:withSetMutation:using:).

### Special Considerations

You rarely need to override this method in subclasses, but if you do, be sure to call `super`.

## See Also

### Notifying Observers of Changes

func willChangeValue(forKey: String)

Informs the observed object that the value of a given property is about to change.

func didChangeValue(forKey: String)

Informs the observed object that the value of a given property has changed.

func willChange(NSKeyValueChange, valuesAt: IndexSet, forKey: String)

Informs the observed object that the specified change is about to be executed at given indexes for a specified ordered to-many relationship.

func didChange(NSKeyValueChange, valuesAt: IndexSet, forKey: String)

Informs the observed object that the specified change has occurred on the indexes for a specified ordered to-many relationship.

func willChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Informs the observed object that the specified change is about to be made to a specified unordered to-many relationship.

