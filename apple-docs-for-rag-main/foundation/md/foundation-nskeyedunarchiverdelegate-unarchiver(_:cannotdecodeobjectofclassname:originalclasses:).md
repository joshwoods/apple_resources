

- Foundation
- NSKeyedUnarchiverDelegate
-  unarchiver(\_:cannotDecodeObjectOfClassName:originalClasses:) 

Instance Method

# unarchiver(\_:cannotDecodeObjectOfClassName:originalClasses:)

Informs the delegate that the class with a given name is not available during decoding.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func unarchiver(
    _ unarchiver: NSKeyedUnarchiver,
    cannotDecodeObjectOfClassName name: String,
    originalClasses classNames: [String]
) -> AnyClass?
```

## Parameters 

`unarchiver`  

An unarchiver for which the receiver is the delegate.

`name`  

The name of the class of an object `unarchiver` is trying to decode.

`classNames`  

An array describing the class hierarchy of the encoded object, where the first element is the class name string of the encoded object, the second element is the class name of its immediate superclass, and so on.

## Return Value

The class unarchiver should use in place of the class named `name`.

## Discussion

The delegate may, for example, load some code to introduce the class to the runtime and return the class, or substitute a different class object. If the delegate returns `nil`, unarchiving aborts and the method raises an `NSInvalidUnarchiveOperationException`.

## See Also

### Related Documentation

Archives and Serializations Programming Guide

### Decoding Objects

func unarchiver(NSKeyedUnarchiver, didDecode: Any?) -> Any?

Informs the delegate that a given object has been decoded.

func unarchiver(NSKeyedUnarchiver, willReplace: Any, with: Any)

Informs the delegate that one object is being substituted for another.

