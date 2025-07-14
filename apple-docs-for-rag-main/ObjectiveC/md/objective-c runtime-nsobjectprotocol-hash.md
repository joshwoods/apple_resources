

- Objective-C Runtime
- NSObjectProtocol
-  hash 

Instance Property

# hash

Returns an integer that can be used as a table address in a hash table structure.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var hash: Int { get }
```

**Required**

## Return Value

An integer that can be used as a table address in a hash table structure.

## Discussion

If two objects are equal (as determined by the isEqual(_:) method), they must have the same hash value. This last point is particularly important if you define hash in a subclass and intend to put instances of that subclass into a collection.

If a mutable object is added to a collection that uses hash values to determine the object’s position in the collection, the value returned by the hash method of the object must not change while the object is in the collection. Therefore, either the hash method must not rely on any of the object’s internal state information or you must make sure the object’s internal state information does not change while the object is in the collection. Thus, for example, a mutable dictionary can be put in a hash table but you must not change it while it is in there. (Note that it can be difficult to know whether or not a given object is in a collection.)

## See Also

### Identifying and Comparing Objects

func isEqual(Any?) -> Bool

Returns a Boolean value that indicates whether the receiver and a given object are equal.

**Required**

func `self`() -> Self

Returns the receiver.

**Required**

