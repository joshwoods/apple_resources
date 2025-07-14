

- WatchKit
-  WKInterfaceSeparator 

Class

# WKInterfaceSeparator

An interface object that displays a visual separator within a group.

watchOS 2.0+

``` source
class WKInterfaceSeparator
```

## Overview

Use WKInterfaceSeparator to manipulate a separator at runtime, such as changing its color. You can also use the inherited methods to show or hide it and configure other attributes.

Do not subclass or create instances of this class yourself. Instead, define outlets in your interface controller class and connect them to the corresponding objects in your storyboard file. For example, to refer to a separator object in your interface, define a property with the following syntax in your interface controller class:

- Swift
- Objective-C

```
@IBOutlet weak var mySeparator: WKInterfaceSeparator!
```

```
@property (weak, nonatomic) IBOutlet WKInterfaceSeparator* mySeparator;
```

During the initialization of your interface controller, WatchKit creates any needed separator objects and assigns them to their connected outlets. At that point, you can use those objects to make changes to the onscreen text.

### Interface Builder Configuration Options

Xcode lets you configure information about your separator interface object in your storyboard file. The following table lists the attributes you can configure and their meaning.

| Attribute | Description |
|----|----|
| Color | The default color of the separator. You can also set this value programmatically using the setColor(_:) method. |

## Topics

### Configuring the Separator

func setColor(UIColor?)

Sets the color of the separator bar.

## Relationships

### Inherits From

- WKInterfaceObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Containers

class WKInterfaceGroup

A container for one or more interface objects.

class WKInterfaceTable

An object that creates and manages the contents of a single-column table interface.

class WKInterfacePicker

An interface element that presents a scrolling list of items for the user to choose from.

