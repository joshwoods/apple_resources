

- AppKit
-  NSColorList 

Class

# NSColorList

An ordered list of color objects, identified by keys.

macOS

``` source
class NSColorList
```

## Overview

A color list manages a list of NSColor objects, each of which has an associated name. The NSColorPanel list mode color picker uses instances of NSColorList to represent any lists of colors that come with the system, as well as any lists the user creates. An app can use a color list to manage document-specific color lists.

## Topics

### Creating Lists of Colors

init(name: NSColorList.Name)

Initializes and returns a color list, registering it under the specified name if it isn’t in use already.

init?(name: NSColorList.Name, fromFile: String?)

Initializes and returns a color list from the specified file, registering it under the specified name if it isn’t in use already.

### Getting Lists of Colors

class var availableColorLists: [NSColorList]

Returns an array of all color lists found in the standard color list directories.

init?(named: NSColorList.Name)

Searches the available color lists array and returns the color list with the specified name.

### Getting Information About Lists of Colors

var name: NSColorList.Name?

The name of the color list.

typealias Name

The name assigned to a color list.

var isEditable: Bool

A Boolean value that indicates whether the color list can be modified.

### Managing Colors By Key

var allKeys: [NSColor.Name]

An array of the keys by which the color objects are stored in the color list.

func color(withKey: NSColor.Name) -> NSColor?

Returns the color object associated with the specified key.

func insertColor(NSColor, key: NSColor.Name, at: Int)

Inserts the specified color at the specified location in the color list.

func removeColor(withKey: NSColor.Name)

Removes the color associated with the specified key from the color list.

func setColor(NSColor, forKey: NSColor.Name)

Associates the specified color object with the specified key.

### Writing and Removing Color List Files

func write(to: URL?) throws

Saves the color list to the file at the specified URL.

func removeFile()

Removes the file from which the list was created, if the file is in a standard search path and owned by the user.

func write(toFile: String?) -> Bool

Saves the color list to the file at the specified path.

Deprecated

### Notifications

class let didChangeNotification: NSNotification.Name

Posted whenever a color list changes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Colors

class NSColor

An object that stores color data and sometimes opacity (alpha value).

class NSColorSpace

An object that represents a custom color space.

