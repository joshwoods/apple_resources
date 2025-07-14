

- Security
-  SecTrustSetOptions(\_:\_:) 

Function

# SecTrustSetOptions(\_:\_:)

Sets option flags for customizing evaluation of a trust object.

macOS 10.7+

``` source
func SecTrustSetOptions(
    _ trustRef: SecTrust,
    _ options: SecTrustOptionFlags
) -> OSStatus
```

## Parameters 

`trustRef`  

The trust object to modify.

`options`  

The new set of option flags. For a list of options, see SecTrustOptionFlags.

## Return Value

A result code. See Security Framework Result Codes.

