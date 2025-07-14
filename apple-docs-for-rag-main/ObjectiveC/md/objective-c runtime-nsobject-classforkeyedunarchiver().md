

- Objective-C Runtime
- NSObject
-  classForKeyedUnarchiver() 

Type Method

# classForKeyedUnarchiver()

Overridden by subclasses to substitute a new class during keyed unarchiving.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func classForKeyedUnarchiver() -> AnyClass
```

## Return Value

The class to substitute for the receiver during keyed unarchiving.

## Discussion

During keyed unarchiving, instances of the receiver will be decoded as members of the returned class. This method overrides the results of the decoder’s class and instance name to class encoding tables.

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

