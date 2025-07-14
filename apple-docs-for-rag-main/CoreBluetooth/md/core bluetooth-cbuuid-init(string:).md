

- Core Bluetooth
- CBUUID
-  init(string:) 

Initializer

# init(string:)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID string.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(string theString: String)
```

## Parameters 

`theString`  

A string containing a 16-, 32-, or 128-bit UUID.

## Return Value

A new CBUUID object for the specified UUID string.

## Discussion

Specify 128-bit UUIDs as a string of hexadecimal digits punctuated by hyphens, for example, 68753A44-4D6F-1226-9C60-0050E4C00067. Specify 16- or 32-bit UUIDs as a string of 4 or 8 hexadecimal digits, respectively. For an example of how to use this method, see Services and Characteristics Are Identified by UUIDs and Create Your Own UUIDs for Custom Services and Characteristics.

For more information, see Core Bluetooth Programming Guide.

## See Also

### Creating New CBUUID Objects

init(data: Data)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID data container.

init(cfuuid: CFUUID)

Creates a Core Bluetooth UUID object from a Core Foundation UUID object.

Deprecated

init(nsuuid: UUID)

Creates a Core Bluetooth UUID object from a Foundation UUID object.

