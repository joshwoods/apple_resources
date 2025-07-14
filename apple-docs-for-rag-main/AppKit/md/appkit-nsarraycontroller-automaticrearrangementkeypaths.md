

- AppKit
- NSArrayController
-  automaticRearrangementKeyPaths 

Instance Property

# automaticRearrangementKeyPaths

An array of key paths that trigger automatic content sorting or filtering

macOS 10.5+

``` source
var automaticRearrangementKeyPaths: [String]? { get }
```

## Discussion

Subclasses can override this property to customize the default behavior of the sort descriptors and filtering predicates, for example, if additional arrangement criteria are used in a custom implementation of arrangedObjects.

## See Also

### Automatic Content Rearranging

var automaticallyRearrangesObjects: Bool

A Boolean that indicates if the receiver automatically rearranges its content to correspond to the current sort descriptors and filter predicates

func didChangeArrangementCriteria()

Invoked when any criteria for arranging objects change.

