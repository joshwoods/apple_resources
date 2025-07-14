

- Contacts
- CNMutableContact
-  dates 

Instance Property

# dates

An array containing labeled Gregorian dates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var dates: [CNLabeledValue] { get set }
```

## Discussion

This property is an array of CNLabeledValue objects, each of which has an NSString label and NSDateComponents value. You can use this property to store Gregorian dates such as anniversaries. Day and month are required and year is optional. Calendar is `nil` or Gregorian. All other date components are invalid.

## See Also

### Setting Birthday Information

var nonGregorianBirthday: DateComponents?

A date component for the non-Gregorian birthday of the contact.

var birthday: DateComponents?

A date component for the Gregorian birthday of the contact.

