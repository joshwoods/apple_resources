

- SceneKit
- SCNTransaction
-  setValue(\_:forKey:) 

Type Method

# setValue(\_:forKey:)

Associates an arbitrary object with the current transaction using the specified key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func setValue(
    _ value: Any?,
    forKey key: String
)
```

## Parameters 

`value`  

An object to associate with the current transaction.

`key`  

A unique string identifying the object for later retrieval.

## Discussion

Nested transactions have nested data scope. Setting a value for a key associates it with the current transaction (or innermost nested transaction) only, and reading the value for a key searches through nested transactions (starting from the innermost).

## See Also

### Getting and Setting Transaction Properties

class func value(forKey: String) -> Any?

Returns the object previously associated with the current transaction using the specified key.

