

- Core WLAN
- CWNetworkProfile
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Determine CWNetworkProfile object equality.

macOS 10.7+

``` source
func isEqual(to networkProfile: CWNetworkProfile) -> Bool
```

## Parameters 

`networkProfile`  

The CWNetworkProfile object with which to compare the receiver.

## Return Value

*YES* if the objects are equal.

## Discussion

CWNetwork objects are considered equal if their corresponding *ssidData* and *securityType* properties are equal.

