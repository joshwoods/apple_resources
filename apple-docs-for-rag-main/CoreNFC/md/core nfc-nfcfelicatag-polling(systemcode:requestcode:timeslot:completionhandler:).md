

- Core NFC
- NFCFeliCaTag
-  polling(systemCode:requestCode:timeSlot:completionHandler:) 

Instance Method

# polling(systemCode:requestCode:timeSlot:completionHandler:)

Sends the Polling command as defined by FeliCa card specification to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func polling(
    systemCode: Data,
    requestCode: NFCFeliCaPollingRequestCode,
    timeSlot: NFCFeliCaPollingTimeSlot,
    completionHandler: @escaping (Data, Data, (any Error)?) -> Void
)
```

``` source
func polling(
    systemCode: Data,
    requestCode: NFCFeliCaPollingRequestCode,
    timeSlot: NFCFeliCaPollingTimeSlot
) async throws -> (Data, Data)
```

**Required**

## See Also

### Polling

typealias PollingRequestCode

Codes that specify the type of the data to request when polling.

Deprecated

typealias PollingTimeSlot

Constants that specify the maximum number of time slots.

Deprecated

