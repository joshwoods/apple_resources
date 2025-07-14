

- Objective-C Runtime
- NSObject
-  replacementObject(for:) Deprecated

Instance Method

# replacementObject(for:)

Overridden by subclasses to substitute another object for itself during archiving.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
func replacementObject(for archiver: NSArchiver) -> Any?
```

## Parameters 

`archiver`  

The archiver creating an archive.

## Return Value

The object to substitute for the receiver during archiving.

## Discussion

This method is invoked by `NSArchiver`. `NSObject`’s implementation returns the object returned by replacementObject(for:).

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

func replacementObject(for: NSCoder) -> Any?

Overridden by subclasses to substitute another object for itself during encoding.

func replacementObject(for: NSKeyedArchiver) -> Any?

Overridden by subclasses to substitute another object for itself during keyed archiving.

class func setVersion(Int)

Sets the receiver’s version number.

class func version() -> Int

Returns the version number assigned to the class.

