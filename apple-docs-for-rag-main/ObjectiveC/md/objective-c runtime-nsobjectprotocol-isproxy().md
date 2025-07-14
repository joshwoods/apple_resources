

- Objective-C Runtime
- NSObjectProtocol
-  isProxy() 

Instance Method

# isProxy()

Returns a Boolean value that indicates whether the receiver does not descend from NSObject.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func isProxy() -> Bool
```

**Required**

## Return Value

NO if the receiver really descends from NSObject, otherwise YES.

## Discussion

This method is necessary because sending isKind(of:) or isMember(of:) to an NSProxy object will test the object the proxy stands in for, not the proxy itself. Use this method to test if the receiver is a proxy (or a member of some other root class).

