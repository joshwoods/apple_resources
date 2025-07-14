

- Objective-C Runtime
- NSObject
-  accessInstanceVariablesDirectly 

Type Property

# accessInstanceVariablesDirectly

Returns a Boolean value that indicates whether the key-value coding methods should access the corresponding instance variable directly on finding no accessor method for a property.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class var accessInstanceVariablesDirectly: Bool { get }
```

## Return Value

YES if the key-value coding methods should access the corresponding instance variable directly on finding no accessor method for a property, otherwise NO.

## Discussion

The default returns YES. Subclasses can override it to return NO, in which case the key-value coding methods won’t access instance variables.

