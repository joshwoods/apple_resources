

- Objective-C Runtime
- NSObject
-  replacementObject(for:) 

Instance Method

# replacementObject(for:)

Overridden by subclasses to substitute another object for itself during keyed archiving.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func replacementObject(for archiver: NSKeyedArchiver) -> Any?
```

## Parameters 

`archiver`  

A keyed archiver creating an archive.

## Return Value

The object encode instead of the receiver (if different).

## Discussion

This method is called only if no replacement mapping for the object has been set up in the encoder (for example, due to a previous call of replacementObject(for:) to that object).

## See Also

### Archiving

func awakeAfter(using: NSCoder) -> Any?

Overridden by subclasses to substitute another object in place of the object that was decoded and subsequently received this message.

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

class func setVersion(Int)

Sets the receiver’s version number.

class func version() -> Int

Returns the version number assigned to the class.

