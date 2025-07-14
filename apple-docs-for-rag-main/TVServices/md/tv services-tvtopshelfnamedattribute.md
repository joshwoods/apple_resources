

- TV Services
-  TVTopShelfNamedAttribute 

Class

# TVTopShelfNamedAttribute

An object you use to display additional information.

tvOS 13.0+

``` source
class TVTopShelfNamedAttribute
```

## Overview

Use TVTopShelfNamedAttribute objects to specify additional information about your content, such as the names of cast or crew members associated with a movie or show. Each named attribute contains the type of information you want to include (the name) and a list of strings (the values) to display for that attribute. For example, you might set the name property to “Starring” and set the value strings to the names of the leading actors.

Create named attributes and assign them to the namedAttributes property of a TVTopShelfCarouselItem object.

## Topics

### Creating a Named Attribute

init(name: String, values: [String])

Creates a new named attribute object with the specified values.

### Getting the Name and Value

var name: String

The localized name of the attribute.

var values: [String]

The array of values for the attribute.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Adding Custom Attributes

var namedAttributes: [TVTopShelfNamedAttribute]

Additional information to display for your content, such as a list of leading actors.

