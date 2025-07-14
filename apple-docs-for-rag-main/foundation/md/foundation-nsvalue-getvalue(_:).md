

- Foundation
- NSValue
-  getValue(\_:) 

Instance Method

# getValue(\_:)

Copies the value into the specified buffer.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func getValue(_ value: UnsafeMutableRawPointer)
```

## Parameters 

`value`  

A buffer into which to copy the value. The buffer must be large enough to hold the value.

## See Also

### Working with Raw Values

init(bytes: UnsafeRawPointer, objCType: UnsafePointer&lt;CChar>)

Initializes a value object to contain the specified value, interpreted with the specified Objective-C type.

init(UnsafeRawPointer, withObjCType: UnsafePointer&lt;CChar>)

Creates a value object containing the specified value, interpreted with the specified Objective-C type.

var objCType: UnsafePointer&lt;CChar>

A C string containing the Objective-C type of the data contained in the value object.

