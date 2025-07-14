

- Core Bluetooth
- CBCharacteristicWriteType
-  CBCharacteristicWriteType.withoutResponse 

Case

# CBCharacteristicWriteType.withoutResponse

Write a characteristic value, without any response from the peripheral to indicate whether the write was successful.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
case withoutResponse
```

## Discussion

You receive no notification if writing to a characteristic value fails with this write type.

## See Also

### Write Types

case withResponse

Write a characteristic value, with a response from the peripheral to indicate whether the write was successful.

