

- Objective-C Runtime
- NSObject
-  replacementObject(for:) 

Instance Method

# replacementObject(for:)

Overridden by subclasses to substitute another object for itself during encoding.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func replacementObject(for coder: NSCoder) -> Any?
```

## Parameters 

`coder`  

The coder encoding the receiver.

## Return Value

The object encode instead of the receiver (if different).

## Discussion

An object might encode itself into an archive, but encode a proxy for itself if it’s being encoded for distribution. This method is invoked by `NSCoder`. `NSObject`’s implementation returns `self`.

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

func replacementObject(for: NSKeyedArchiver) -> Any?

Overridden by subclasses to substitute another object for itself during keyed archiving.

class func setVersion(Int)

Sets the receiver’s version number.

class func version() -> Int

Returns the version number assigned to the class.

