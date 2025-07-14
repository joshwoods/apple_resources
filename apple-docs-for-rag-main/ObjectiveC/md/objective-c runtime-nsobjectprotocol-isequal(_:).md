

- Objective-C Runtime
- NSObjectProtocol
-  isEqual(\_:) 

Instance Method

# isEqual(\_:)

Returns a Boolean value that indicates whether the receiver and a given object are equal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func isEqual(_ object: Any?) -> Bool
```

**Required**

## Parameters 

`object`  

The object to be compared to the receiver. May be `nil`, in which case this method returns NO.

## Return Value

YES if the receiver and `anObject` are equal, otherwise NO.

## Discussion

This method defines what it means for instances to be equal. For example, a container object might define two containers as equal if their corresponding objects all respond YES to an isEqual(_:) request. See the NSData, NSDictionary, NSArray, and NSString class specifications for examples of the use of this method.

If two objects are equal, they must have the same hash value. This last point is particularly important if you define isEqual(_:) in a subclass and intend to put instances of that subclass into a collection. Make sure you also define hash in your subclass.

## See Also

### Identifying and Comparing Objects

var hash: Int

Returns an integer that can be used as a table address in a hash table structure.

**Required**

func `self`() -> Self

Returns the receiver.

**Required**

