

- IOBluetooth
- IOBluetoothHandsFree
-  setIndicator(\_:value:) 

Instance Method

# setIndicator(\_:value:)

Set an indicator’s value

macOS 10.7+

``` source
func setIndicator(
    _ indicatorName: String!,
    value indicatorValue: Int32
)
```

## Parameters 

`indicatorName`  

See “Hands free indicator constants,” for standard indicator names.

`indicatorValue`  

Will set the indicator value as long as it is within the min and max values allowed.

## Discussion

Sets an indicator’s value.

