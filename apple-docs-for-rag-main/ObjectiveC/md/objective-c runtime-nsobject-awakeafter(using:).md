

- Objective-C Runtime
- NSObject
-  awakeAfter(using:) 

Instance Method

# awakeAfter(using:)

Overridden by subclasses to substitute another object in place of the object that was decoded and subsequently received this message.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func awakeAfter(using coder: NSCoder) -> Any?
```

## Parameters 

`coder`  

The decoder used to decode the receiver.

## Return Value

The receiver, or another object to take the place of the object that was decoded and subsequently received this message.

## Discussion

You can use this method to eliminate redundant objects created by the coder. For example, if after decoding an object you discover that an equivalent object already exists, you can return the existing object. If a replacement is returned, your overriding method is responsible for releasing the receiver.

This method is invoked by `NSCoder`. `NSObject`’s implementation simply returns `self`.

## See Also

### Related Documentation

init?(coder: NSCoder)

### Archiving

var classForArchiver: AnyClass?

The class to substitute for the receiver’s own class during archiving.

var classForCoder: AnyClass

Overridden by subclasses to substitute a class other than its own during coding.

var classForKeyedArchiver: AnyClass?

Subclasses to substitute a new class for instances during keyed archiving.

class func classFallbacksForKeyedArchiver() -> [String]

Overridden to return the names of classes that can be used to decode objects if their class is unavailable.

class func classForKeyedUnarchiver() -> AnyClass

Overridden by subclasses to substitute a new class during keyed unarchiving.

func replacementObject(for: NSArchiver) -> Any?

Overridden by subclasses to substitute another object for itself during archiving.

Deprecated

func replacementObject(for: NSCoder) -> Any?

Overridden by subclasses to substitute another object for itself during encoding.

func replacementObject(for: NSKeyedArchiver) -> Any?

Overridden by subclasses to substitute another object for itself during keyed archiving.

class func setVersion(Int)

Sets the receiver’s version number.

class func version() -> Int

Returns the version number assigned to the class.

