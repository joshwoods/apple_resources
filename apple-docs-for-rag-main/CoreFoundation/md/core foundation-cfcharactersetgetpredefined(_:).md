

- Core Foundation
-  CFCharacterSetGetPredefined(\_:) 

Function

# CFCharacterSetGetPredefined(\_:)

Returns a predefined character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetGetPredefined(_ theSetIdentifier: CFCharacterSetPredefinedSet) -> CFCharacterSet!
```

## Parameters 

`theSetIdentifier`  

A predefined character set. See Predefined CFCharacterSet Selector Values for the list of available character sets.

## Return Value

A predefined character set. This instance is owned by Core Foundation.

