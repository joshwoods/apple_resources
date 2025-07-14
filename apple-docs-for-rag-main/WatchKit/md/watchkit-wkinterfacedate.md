

- WatchKit
-  WKInterfaceDate 

Class

# WKInterfaceDate

A label that displays the current date or time.

watchOS 2.0+

``` source
class WKInterfaceDate
```

## Overview

Use WKInterfaceDate when you want to display date or time information without further interaction from your WatchKit extension. At runtime, use the date object to configure the appearance of the date and time information being displayed.

Do not subclass or create instances of this class yourself. Instead, define outlets in your interface controller class and connect them to the corresponding objects in your storyboard file. For example, to refer to a date object in your interface, define a property with the following syntax in your interface controller class:

- Swift
- Objective-C

```
@IBOutlet weak var myDate: WKInterfaceDate!
```

```
@property (weak, nonatomic) IBOutlet WKInterfaceDate* myDate;
```

During the initialization of your interface controller, WatchKit creates any needed date objects and assigns them to their connected outlets. After those objects are set, you can use them to make changes to the onscreen date and time information.

### Interface Builder Configuration Options

Xcode lets you configure information about your date interface object in your storyboard file. The following table lists the attributes you can configure and their meaning.

| Attribute | Description |
|----|----|
| Format | A selector for choosing between standard and custom formats. For standard formats, you use the Date and Time attributes to configure the information you want to display. Changing the value of this attribute to Custom lets you configure the date exactly the way you want based on the format options described in Data Formatting Guide. |
| Date | The date information to display. The date options correspond to the values of the DateFormatter.Style type. |
| Time | The time information to display. The time options correspond to the values of the DateFormatter.Style type. |
| Preview | A preview of what the date and time will look like. |

A date object is a custom label whose text you cannot set directly. However, you can customize the appearance of the date object as you would customize a label using the Attributes inspector in Xcode. For information about the label attributes you can configure, see WKInterfaceLabel.

## Topics

### Configuring the Date and Time Display

func setTextColor(UIColor?)

Sets the color of the date and time text.

func setTimeZone(TimeZone?)

Sets the time zone to use when displaying time information.

func setCalendar(Calendar?)

Sets the calendar to use when formatting date information.

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

### Controls

class WKInterfaceLabel

An interface element that displays static text.

class WKInterfaceTimer

A label that displays a countdown or count-up timer.

class WKInterfaceButton

A button in the user interface of your watchOS app.

class WKInterfaceAuthorizationAppleIDButton

A button that you can use to trigger a Sign in with Apple request.

class WKInterfacePaymentButton

A button that you can use to trigger payments through Apple Pay.

class WKInterfaceTextField

An interface element that displays an editable text area.

class WKInterfaceSwitch

An interface element that toggles between an On and Off state.

class WKInterfaceSlider

An interface element that lets users select a single floating-point value from a range of values.

class WKInterfaceActivityRing

A view that displays data from a HealthKit activity summary object.

class WKInterfaceMap

An interface element that displays a noninteractive map for the location you specify.

