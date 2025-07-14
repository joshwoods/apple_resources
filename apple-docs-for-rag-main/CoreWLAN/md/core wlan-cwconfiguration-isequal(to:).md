

- Core WLAN
- CWConfiguration
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Determine CWConfiguration object equality.

macOS 10.6+

``` source
func isEqual(to configuration: CWConfiguration) -> Bool
```

## Parameters 

`configuration`  

The CWConfiguration object with which to compare the receiver.

## Return Value

*YES* if the objects are equal.

## Discussion

CWConfiguration objects are considered equal if all their corresponding properties are equal.

