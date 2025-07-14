

- SceneKit
-  SCNConsistencyElementIDErrorKey 

Global Variable

# SCNConsistencyElementIDErrorKey

The identifier of the scene file element where the error occurred.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let SCNConsistencyElementIDErrorKey: String
```

## Discussion

The value for this key is a NSString object containing an identifier.

If the element in which the error occurred does not have an identifier, the value for this key is the identifier of the closest parent element with an identifier.

## See Also

### Constants

let SCNConsistencyElementTypeErrorKey: String

The type of scene file element in which the error occurred.

let SCNConsistencyLineNumberErrorKey: String

The line number in the scene file in which the error occurred.

