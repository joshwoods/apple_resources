

- Core NFC
- NFCFeliCaTag
-  polling(systemCode:requestCode:timeSlot:resultHandler:) 

Instance Method

# polling(systemCode:requestCode:timeSlot:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func polling(
    systemCode: Data,
    requestCode: NFCFeliCaPollingRequestCode,
    timeSlot: NFCFeliCaPollingTimeSlot,
    resultHandler: @escaping (Result) -> Void
)
```

