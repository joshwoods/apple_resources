

- Foundation
- DateFormatter
-  localizedString(from:dateStyle:timeStyle:) 

Type Method

# localizedString(from:dateStyle:timeStyle:)

Returns a string representation of a specified date, that the system formats for the current locale using the specified date and time styles.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func localizedString(
    from date: Date,
    dateStyle dstyle: DateFormatter.Style,
    timeStyle tstyle: DateFormatter.Style
) -> String
```

## Parameters 

`date`  

A date.

`dstyle`  

A format style for the date. For possible values, see DateFormatter.Style.

`tstyle`  

A format style for the time. For possible values, see DateFormatter.Style.

## Return Value

A localized string representation of `date` using the specified date and time styles.

## Discussion

This method uses a date formatter configured with the current default settings. The returned string is the same as if you configured and used a date formatter as shown in the following example:

```
NSDateFormatter *formatter = [[NSDateFormatter alloc] init];
formatter.formatterBehavior = NSDateFormatterBehavior10_4;
formatter.dateStyle = dateStyle;
formatter.timeStyle = timeStyle;
NSString *result = [formatter stringForObjectValue:date];
```

## See Also

### Converting Objects

func date(from: String) -> Date?

Returns a date representation of a specified string that the system interprets using the receiver’s current settings.

func string(from: Date) -> String

Returns a string representation of a specified date that the system formats using the receiver’s current settings.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, range: UnsafeMutablePointer&lt;NSRange>?) throws

Returns by reference a date representation of a specified string and its date range, as well as a Boolean value that indicates whether the system can parse the string.

