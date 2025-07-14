

- AppKit
- NSArrayController
-  didChangeArrangementCriteria() 

Instance Method

# didChangeArrangementCriteria()

Invoked when any criteria for arranging objects change.

macOS 10.5+

``` source
func didChangeArrangementCriteria()
```

## Discussion

This method is invoked by the controller itself when any criteria for arranging objects change (sort descriptors or filter predicates) to reset the key paths for automatic rearranging.

### Special Considerations

If you implement a subclass of `NSArrayController` and override rearrangeObjects() to use additional arrangement criteria, you should invoke this method if those criteria change.

## See Also

### Related Documentation

func rearrangeObjects()

Triggers filtering of the receiver’s content.

### Automatic Content Rearranging

var automaticallyRearrangesObjects: Bool

A Boolean that indicates if the receiver automatically rearranges its content to correspond to the current sort descriptors and filter predicates

var automaticRearrangementKeyPaths: [String]?

An array of key paths that trigger automatic content sorting or filtering

