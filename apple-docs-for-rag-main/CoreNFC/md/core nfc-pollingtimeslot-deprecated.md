

- Core NFC
-  PollingTimeSlot Deprecated

Type Alias

# PollingTimeSlot

Constants that specify the maximum number of time slots.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
typealias PollingTimeSlot = NFCFeliCaPollingTimeSlot
```

## Topics

### Maximum Slots

static var PollingTimeSlotMax1: NFCFeliCaPollingTimeSlot

A constant that indicates a maximum of one slot.

static var PollingTimeSlotMax2: NFCFeliCaPollingTimeSlot

A constant that indicates a maximum of two slots.

static var PollingTimeSlotMax4: NFCFeliCaPollingTimeSlot

A constant that indicates a maximum of four slots.

static var PollingTimeSlotMax8: NFCFeliCaPollingTimeSlot

A constant that indicates a maximum of eight slots.

static var PollingTimeSlotMax16: NFCFeliCaPollingTimeSlot

A constant that indicates a maximum of sixteen slots.

## See Also

### Polling

func polling(systemCode: Data, requestCode: NFCFeliCaPollingRequestCode, timeSlot: NFCFeliCaPollingTimeSlot, completionHandler: (Data, Data, (any Error)?) -> Void)

Sends the Polling command as defined by FeliCa card specification to the tag.

**Required**

typealias PollingRequestCode

Codes that specify the type of the data to request when polling.

Deprecated

