

- Core Text
-  CTParagraphStyleSetting 

Structure

# CTParagraphStyleSetting

This structure is used to alter the paragraph style.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTParagraphStyleSetting
```

## Topics

### Initializers

init(spec: CTParagraphStyleSpecifier, valueSize: Int, value: UnsafeRawPointer)

### Instance Properties

var spec: CTParagraphStyleSpecifier

The specifier of the setting. See CTParagraphStyleSpecifier for possible values.

var value: UnsafeRawPointer

A reference to the value of the setting specified by the `spec` field. The value must be in the proper range for the `spec` value and at least as large as the size specified in `valueSize`.

var valueSize: Int

The size of the value pointed to by the `value` field. This value must match the size of the value required by the `CTParagraphStyleSpecifier` set in the `spec` field.

## Relationships

### Conforms To

- BitwiseCopyable

