

- UIKit
- UIStateRestoring
-  objectRestorationClass 

Instance Property

# objectRestorationClass

The class responsible for creating this object when restoring the app’s state.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var objectRestorationClass: (any UIObjectRestoration.Type)? { get }
```

## Discussion

If an object has an associated restoration class, the object(withRestorationIdentifierPath:coder:) method of that class is called during state restoration. That method is responsible for returning the object that matches the provided path identifier information. If this property is`nil`, the object must already exist and be registered with the state restoration engine so that it can be found implicitly. You can register the object using the registerObject(forStateRestoration:restorationIdentifier:) method at launch time.

The restoration class must conform to the UIObjectRestoration protocol.

## See Also

### Accessing the object information

var restorationParent: (any UIStateRestoring)?

The parent object used to scope the current object.

