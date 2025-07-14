

- UIKit
- UIStateRestoring
-  restorationParent 

Instance Property

# restorationParent

The parent object used to scope the current object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var restorationParent: (any UIStateRestoring)? { get }
```

## Discussion

Returning an object from this property lets you use the same restoration identifier for objects with similar behavior but different parents. When registering objects, the registerObject(forStateRestoration:restorationIdentifier:) method checks the value of this property, using the value as the containing scope for the object. For example, an object associated with a view controller can make the view controller its parent.

## See Also

### Accessing the object information

var objectRestorationClass: (any UIObjectRestoration.Type)?

The class responsible for creating this object when restoring the app’s state.

