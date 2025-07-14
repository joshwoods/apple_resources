

- AppKit
- NSArrayController
-  automaticallyRearrangesObjects 

Instance Property

# automaticallyRearrangesObjects

A Boolean that indicates if the receiver automatically rearranges its content to correspond to the current sort descriptors and filter predicates

macOS 10.5+

``` source
var automaticallyRearrangesObjects: Bool { get set }
```

## Discussion

The default is false.

## See Also

### Automatic Content Rearranging

var automaticRearrangementKeyPaths: [String]?

An array of key paths that trigger automatic content sorting or filtering

func didChangeArrangementCriteria()

Invoked when any criteria for arranging objects change.

