

- Objective-C Runtime
- NSObject
-  addObserver(\_:forKeyPath:options:context:) 

Instance Method

# addObserver(\_:forKeyPath:options:context:)

Registers the observer object to receive KVO notifications for the key path relative to the object receiving this message.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func addObserver(
    _ observer: NSObject,
    forKeyPath keyPath: String,
    options: NSKeyValueObservingOptions = [],
    context: UnsafeMutableRawPointer?
)
```

## Parameters 

`observer`  

The object to register for KVO notifications. The observer must implement the key-value observing method observeValue(forKeyPath:of:change:context:).

`keyPath`  

The key path, relative to the object receiving this message, of the property to observe. This value must not be `nil`.

`options`  

A combination of the `NSKeyValueObservingOptions` values that specifies what is included in observation notifications. For possible values, see NSKeyValueObservingOptions.

`context`  

Arbitrary data that is passed to `observer` in observeValue(forKeyPath:of:change:context:).

## Discussion

Neither the object receiving this message, nor `observer`, are retained. An object that calls this method must also eventually call either the removeObserver(_:forKeyPath:) or removeObserver(_:forKeyPath:context:) method to unregister the observer when participating in KVO.

## See Also

### Registering for Observation

func removeObserver(NSObject, forKeyPath: String)

Stops the observer object from receiving change notifications for the property specified by the key path relative to the object receiving this message.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Stops the observer object from receiving change notifications for the property specified by the key path relative to the object receiving this message, given the context.

