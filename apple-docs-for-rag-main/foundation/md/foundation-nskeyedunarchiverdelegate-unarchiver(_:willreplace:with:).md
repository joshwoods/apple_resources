

- Foundation
- NSKeyedUnarchiverDelegate
-  unarchiver(\_:willReplace:with:) 

Instance Method

# unarchiver(\_:willReplace:with:)

Informs the delegate that one object is being substituted for another.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func unarchiver(
    _ unarchiver: NSKeyedUnarchiver,
    willReplace object: Any,
    with newObject: Any
)
```

## Parameters 

`unarchiver`  

An unarchiver for which the receiver is the delegate.

`object`  

An object in the archive.

`newObject`  

The object with which `unarchiver` will replace `object`.

## Discussion

This method is called even when the delegate itself is doing, or has done, the substitution with unarchiver(_:didDecode:).

The delegate may use this method if it is keeping track of the encoded or decoded objects.

## See Also

### Decoding Objects

func unarchiver(NSKeyedUnarchiver, cannotDecodeObjectOfClassName: String, originalClasses: [String]) -> AnyClass?

Informs the delegate that the class with a given name is not available during decoding.

func unarchiver(NSKeyedUnarchiver, didDecode: Any?) -> Any?

Informs the delegate that a given object has been decoded.

