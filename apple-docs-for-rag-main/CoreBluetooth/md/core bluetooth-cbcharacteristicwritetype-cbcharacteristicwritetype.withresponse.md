

- Core Bluetooth
- CBCharacteristicWriteType
-  CBCharacteristicWriteType.withResponse 

Case

# CBCharacteristicWriteType.withResponse

Write a characteristic value, with a response from the peripheral to indicate whether the write was successful.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
case withResponse
```

## Discussion

If the write is unsuccessful, the peripheral responds with an error that details the cause of the failure.

## See Also

### Write Types

case withoutResponse

Write a characteristic value, without any response from the peripheral to indicate whether the write was successful.

