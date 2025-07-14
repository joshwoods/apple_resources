

- Core Bluetooth
- CBUUID
-  init(cfuuid:) Deprecated

Initializer

# init(cfuuid:)

Creates a Core Bluetooth UUID object from a Core Foundation UUID object.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.13DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
init(cfuuid theUUID: CFUUID)
```

## Parameters 

`theUUID`  

A UUID represented by a CFUUID object.

## Return Value

A new CBUUID object for the specified UUID.

## See Also

### Creating New CBUUID Objects

init(string: String)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID string.

init(data: Data)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID data container.

init(nsuuid: UUID)

Creates a Core Bluetooth UUID object from a Foundation UUID object.

