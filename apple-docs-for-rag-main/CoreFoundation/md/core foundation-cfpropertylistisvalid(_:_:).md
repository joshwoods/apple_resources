

- Core Foundation
-  CFPropertyListIsValid(\_:\_:) 

Function

# CFPropertyListIsValid(\_:\_:)

Determines if a property list is valid.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPropertyListIsValid(
    _ plist: CFPropertyList!,
    _ format: CFPropertyListFormat
) -> Bool
```

## Parameters 

`plist`  

The property list to validate.

`format`  

A constant that specifies the allowable format of `plist`. See CFPropertyListFormat for possible values.

## Return Value

`true` if the object graph rooted at `plist` is a valid property list graph—that is, the property list contains no cycles, only contains property list objects, and all dictionary keys are strings; otherwise `false`.

## Discussion

The debugging library version of this function prints out some useful messages.

