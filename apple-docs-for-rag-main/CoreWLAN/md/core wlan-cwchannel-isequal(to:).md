

- Core WLAN
- CWChannel
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Determine CWChannel object equality.

macOS 10.7+

``` source
func isEqual(to channel: CWChannel) -> Bool
```

## Parameters 

`channel`  

The CWChannel object with which to compare the receiver.

## Return Value

*YES* if the objects are equal.

## Discussion

CWChannel objects are considered equal if all their corresponding properties are equal.

