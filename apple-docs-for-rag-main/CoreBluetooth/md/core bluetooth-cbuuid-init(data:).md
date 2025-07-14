

- Core Bluetooth
- CBUUID
-  init(data:) 

Initializer

# init(data:)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID data container.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(data theData: Data)
```

## Parameters 

`theData`  

Data containing a 16-, 32-, or 128-bit UUID.

## Return Value

A new CBUUID object for the specified UUID data.

## Discussion

This method is useful when handling the UUID of a Bluetooth attribute in raw bytes.

## See Also

### Creating New CBUUID Objects

init(string: String)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID string.

init(cfuuid: CFUUID)

Creates a Core Bluetooth UUID object from a Core Foundation UUID object.

Deprecated

init(nsuuid: UUID)

Creates a Core Bluetooth UUID object from a Foundation UUID object.

