

- Objective-C Runtime
- NSObject
-  description() 

Type Method

# description()

Returns a string that represents the contents of the receiving class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func description() -> String
```

## Return Value

A string that represents the contents of the receiving class.

## Discussion

The debugger’s print-object command invokes this method to produce a textual description of an object.

`NSObject`’s implementation of this method simply prints the name of the class.

## See Also

### Related Documentation

var description: String

A textual representation of the receiver.

**Required**

