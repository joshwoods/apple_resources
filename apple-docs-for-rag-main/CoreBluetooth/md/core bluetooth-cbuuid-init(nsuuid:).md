

- Core Bluetooth
- CBUUID
-  init(nsuuid:) 

Initializer

# init(nsuuid:)

Creates a Core Bluetooth UUID object from a Foundation UUID object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(nsuuid theUUID: UUID)
```

## Parameters 

`theUUID`  

A UUID represented by an NSUUID object.

## Return Value

A new CBUUID object for the specified UUID.

## See Also

### Creating New CBUUID Objects

init(string: String)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID string.

init(data: Data)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID data container.

init(cfuuid: CFUUID)

Creates a Core Bluetooth UUID object from a Core Foundation UUID object.

Deprecated

