

- Objective-C Runtime
- NSObject
-  observationInfo 

Instance Property

# observationInfo

Returns a pointer that identifies information about all of the observers that are registered with the observed object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var observationInfo: UnsafeMutableRawPointer? { get set }
```

## Return Value

A pointer that identifies information about all of the observers that are registered with the observed object, the options that were used at registration-time, and so on.

## Discussion

The default implementation of this method retrieves the information from a global dictionary of observed objects keyed by memory addresses.

For improved performance, both this property and observationInfo can be overridden to store the opaque data pointer in an instance variable. Overrides of this property must not attempt to send messages to the stored data.

## See Also

### Observing Customization

class func automaticallyNotifiesObservers(forKey: String) -> Bool

Returns a Boolean value that indicates whether the observed object supports automatic key-value observation for the given key.

class func keyPathsForValuesAffectingValue(forKey: String) -> Set&lt;String>

Returns a set of key paths for properties whose values affect the value of the specified key.

