

- Objective-C Runtime
- NSObjectProtocol
-  isMember(of:) 

Instance Method

# isMember(of:)

Returns a Boolean value that indicates whether the receiver is an instance of a given class.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func isMember(of aClass: AnyClass) -> Bool
```

**Required**

## Parameters 

`aClass`  

A class object representing the Objective-C class to be tested.

## Return Value

YES if the receiver is an instance of `aClass`, otherwise NO.

## Discussion

For example, in this code, isMember(of:) would return NO:

```
NSMutableData *myData = [NSMutableData dataWithCapacity:30];
id anArchiver = [[NSArchiver alloc] initForWritingWithMutableData:myData];
if ([anArchiver isMemberOfClass:[NSCoder class]])
    ...
```

Class objects may be compiler-created objects but they still support the concept of membership. Thus, you can use this method to verify that the receiver is a specific Class object.

## See Also

### Testing Object Inheritance, Behavior, and Conformance

func isKind(of: AnyClass) -> Bool

Returns a Boolean value that indicates whether the receiver is an instance of given class or an instance of any class that inherits from that class.

**Required**

func responds(to: Selector!) -> Bool

Returns a Boolean value that indicates whether the receiver implements or inherits a method that can respond to a specified message.

**Required**

func conforms(to: Protocol) -> Bool

Returns a Boolean value that indicates whether the receiver conforms to a given protocol.

**Required**

