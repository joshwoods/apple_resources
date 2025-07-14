

- AppKit
-  NSFontCollection 

Class

# NSFontCollection

A font collection, which is a group of font descriptors taken together as a single object.

macOS 10.7+

``` source
class NSFontCollection
```

## Overview

You can publicize the font collection as a named collection and it is presented through the System user interface such as the font panel and Font Book. The queries can be modified using the NSMutableFontCollection subclass.

## Topics

### Creating Font Collections

init(descriptors: [NSFontDescriptor])

Returns a font collection matching the given descriptors.

init?(locale: Locale)

Returns a collection of fonts matching the given locale.

init?(name: NSFontCollection.Name)

Creates a named font collection object.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a font collection with the specified name and font visibility.

class var withAllAvailableDescriptors: NSFontCollection

The font collection that matches all registered fonts.

### Naming the Font Collection

class func rename(fromName: NSFontCollection.Name, visibility: NSFontCollection.Visibility, toName: NSFontCollection.Name) throws

Renames the font collection with the specified name and visibility to the second name specified.

class func show(NSFontCollection, withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Make the given font collection visible by giving it a name.

class func hide(withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Remove from view the named font collection with the specified visibility.

class var allFontCollectionNames: [NSFontCollection.Name]

Returns all named collections visible to this process.

struct Name

The constants represent the standard mutable collection names—these names are included in the list of allFontCollectionNames–they have special meaning to the Cocoa font system and should not be hidden or renamed.

struct Visibility

Constants that specify the visibility of font collections.

### Getting the Font Descriptors

var matchingDescriptors: [NSFontDescriptor]?

An array of font descriptors matching the logical descriptors.

func matchingDescriptors(forFamily: String) -> [NSFontDescriptor]?

Returns an array of font descriptors matching the logical descriptors for the given font family.

func matchingDescriptors(forFamily: String, options: [NSFontCollectionMatchingOptionKey : NSNumber]?) -> [NSFontDescriptor]?

Returns an array of font descriptors matching the logical descriptors for the given font family and options.

func matchingDescriptors(options: [NSFontCollectionMatchingOptionKey : NSNumber]?) -> [NSFontDescriptor]?

Returns an array of font descriptors matching the logical descriptors with the given options.

struct NSFontCollectionMatchingOptionKey

These constants are used by the matchingDescriptors(options:) and matchingDescriptors(forFamily:options:) options dictionary parameters.

var queryDescriptors: [NSFontDescriptor]?

An array of font descriptors whose matching results produce the collection’s matching descriptors.

var exclusionDescriptors: [NSFontDescriptor]?

A list of query font descriptors whose matching results are excluded from the list of matching descriptors.

### Responding to Changes

class let didChangeNotification: NSNotification.Name

Posted whenever a font collection is changed.

struct UserInfoKey

These constants are used as keys in the didChangeNotification `userInfo` dictionary to indicate the changes that have taken place.

struct ActionTypeKey

The following actions are possible values of the actionUserInfoKey in the didChangeNotification `userInfo` method.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSMutableFontCollection

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Management

class NSFontManager

The center of activity for the font-conversion system.

class NSMutableFontCollection

A mutable collection of font descriptors taken together as a single object.

struct NSFontCollectionOptions

Constants that support font collection management.

