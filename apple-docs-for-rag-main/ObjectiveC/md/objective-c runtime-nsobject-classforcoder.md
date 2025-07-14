

- Objective-C Runtime
- NSObject
-  classForCoder 

Instance Property

# classForCoder

Overridden by subclasses to substitute a class other than its own during coding.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var classForCoder: AnyClass { get }
```

## Discussion

This method is invoked by `NSCoder`. `NSObject`‘s implementation returns the receiver’s class. The private subclasses of a class cluster substitute the name of their public superclass when being archived.

## See Also

### Archiving

func awakeAfter(using: NSCoder) -> Any?

Overridden by subclasses to substitute another object in place of the object that was decoded and subsequently received this message.

var classForArchiver: AnyClass?

The class to substitute for the receiver’s own class during archiving.

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

