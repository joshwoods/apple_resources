

- Core WLAN
- CWNetwork
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Method for determining CWNetwork object equality.

macOS 10.6+

``` source
func isEqual(to network: CWNetwork) -> Bool
```

## Parameters 

`network`  

The CWNetwork object for which to test equality.

## Return Value

*YES* if the objects are equal.

## Discussion

Two CWNetwork objects are considered equal if their corresponding *ssidData*, *securityType*, and *networkType* properties are equal.

