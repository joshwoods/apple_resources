

- SceneKit
- SCNTransaction
-  value(forKey:) 

Type Method

# value(forKey:)

Returns the object previously associated with the current transaction using the specified key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func value(forKey key: String) -> Any?
```

## Parameters 

`key`  

The unique string identifying an object previously associated with the transaction.

## Return Value

The object previously associated with the transaction (or an enclosing transaction) using the specified key, or `nil` if no value for that key could be found.

## Discussion

Nested transactions have nested data scope. Setting a value for a key associates it with the current transaction (or innermost nested transaction) only, but reading the value for a key searches through nested transactions (starting from the innermost).

## See Also

### Getting and Setting Transaction Properties

class func setValue(Any?, forKey: String)

Associates an arbitrary object with the current transaction using the specified key.

