

- Scripting Bridge
-  SBObject 

Class

# SBObject

The `SBObject` class declares methods that can be invoked on any object in a scriptable application. It defines methods for getting elements and properties of an object, as well as setting a given object to a new value.

Mac Catalyst 13.0+macOS 10.5+

``` source
class SBObject
```

## Overview

Each `SBObject` is built around an object specifier, which tells Scripting Bridge how to locate the object. Therefore, you can think of an `SBObject` as a reference to an object in an target application rather than an object itself. To bypass this reference-based approach and force evaluation, use the get() method.

Typically, rather than create `SBObject` instances explictly, you receive `SBObject` objects by calling methods of an SBApplication subclass. For example, if you wanted to get an `SBObject` representing the current iTunes track, you would use code like this (where `iTunesTrack` is a subclass of `SBObject`):

```
iTunesApplication *iTunes = [SBApplication applicationWithBundleIdentifier:@"com.apple.iTunes"];
iTunesTrack *track = [iTunes currentTrack];
```

You can discover the names of dynamically generated classes such as `iTunesApplication` and `iTunesTrack` by examining the header file created by the `sdp` tool. Alternatively, you give these variables the dynamic Objective-C type `id`.

## Topics

### Initializing a Scripting Bridge Object

init()

Initializes and returns an instance of an `SBObject` subclass.

init(data: Any)

Returns an instance of an `SBObject` subclass initialized with the given data.

init(properties: [AnyHashable : Any])

Returns an instance of an `SBObject` subclass initialized with the specified properties.

init(elementCode: DescType, properties: [String : Any]?, data: Any?)

Returns an instance of an `SBObject` subclass initialized with the specified properties and data and added to the designated element array.

### Getting Referenced Data

func get() -> Any?

Forces evaluation of the receiver, causing the real object to be returned immediately.

### Sending Apple Events

func setTo(Any?)

Sets the receiver to a specified value.

### Getting Properties and Elements

func property(with: AnyClass, code: AEKeyword) -> SBObject

Returns an object of the designated scripting class representing the specified property of the receiver

func property(withCode: AEKeyword) -> SBObject

Returns an object representing the specified property of the receiver.

func elementArray(withCode: DescType) -> SBElementArray

Returns an array containing every child of the receiver with the given class-type code.

### Instance Methods

func lastError() -> (any Error)?

The error from the last event this object sent, or nil if it succeeded.

## Relationships

### Inherits From

- NSObject

### Inherited By

- SBApplication

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

