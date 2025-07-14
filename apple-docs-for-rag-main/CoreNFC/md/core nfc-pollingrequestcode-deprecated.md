

- Core NFC
-  PollingRequestCode Deprecated

Type Alias

# PollingRequestCode

Codes that specify the type of the data to request when polling.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
typealias PollingRequestCode = NFCFeliCaPollingRequestCode
```

## Topics

### Request Codes

static var PollingRequestCodeNoRequest: NFCFeliCaPollingRequestCode

A code that indicates no request.

static var PollingRequestCodeSystemCode: NFCFeliCaPollingRequestCode

A code that indicates a system code request.

static var PollingRequestCodeCommunicationPerformance: NFCFeliCaPollingRequestCode

A code that indicates a communication performance request.

## See Also

### Polling

func polling(systemCode: Data, requestCode: NFCFeliCaPollingRequestCode, timeSlot: NFCFeliCaPollingTimeSlot, completionHandler: (Data, Data, (any Error)?) -> Void)

Sends the Polling command as defined by FeliCa card specification to the tag.

**Required**

typealias PollingTimeSlot

Constants that specify the maximum number of time slots.

Deprecated

