

- Objective-C Runtime
- NSObject
-  automaticallyNotifiesObservers(forKey:) 

Type Method

# automaticallyNotifiesObservers(forKey:)

Returns a Boolean value that indicates whether the observed object supports automatic key-value observation for the given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func automaticallyNotifiesObservers(forKey key: String) -> Bool
```

## Return Value

YES if the key-value observing machinery should automatically invoke willChangeValue(forKey:)/didChangeValue(forKey:) and willChange(_:valuesAt:forKey:)/didChange(_:valuesAt:forKey:) whenever instances of the class receive key-value coding messages for the `key`, or mutating key-value-coding-compliant methods for the `key` are invoked; otherwise NO.

## Discussion

The default implementation returns YES. Starting in OS X 10.5, the default implementation of this method searches the receiving class for a method whose name matches the pattern `+automaticallyNotifiesObserversOf`, and returns the result of invoking that method if it is found. Any found methods must return `BOOL`. If no such method is found YES is returned.

## See Also

### Observing Customization

class func keyPathsForValuesAffectingValue(forKey: String) -> Set&lt;String>

Returns a set of key paths for properties whose values affect the value of the specified key.

var observationInfo: UnsafeMutableRawPointer?

Returns a pointer that identifies information about all of the observers that are registered with the observed object.

