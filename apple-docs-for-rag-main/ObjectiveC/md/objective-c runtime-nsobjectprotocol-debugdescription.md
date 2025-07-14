

- Objective-C Runtime
- NSObjectProtocol
-  debugDescription 

Instance Property

# debugDescription

A textual representation of the receiver to use with a debugger.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
optional var debugDescription: String { get }
```

## Return Value

A string that describes the object for debugging purposes.

## Discussion

The debugger’s `po` command uses this property to create a textual representation of the object suitable for display in the debugger. The default implemention returns the same value as description. Override either property to provide custom object descriptions.

## See Also

### Describing Objects

var description: String

A textual representation of the receiver.

**Required**

