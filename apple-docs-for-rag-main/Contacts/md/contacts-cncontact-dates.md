

- Contacts
- CNContact
-  dates 

Instance Property

# dates

An array containing labeled Gregorian dates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var dates: [CNLabeledValue] { get }
```

## Discussion

This property is an array of CNLabeledValue objects, each of which has an NSString label and NSDateComponents value. You can use this property to store Gregorian dates such as anniversaries. Day and month components are required and year is optional. The calendar component can be `nil` or gregorian. All other date components are invalid and including them results in an NSError object that includes the key paths of the invalid components and the error code CNError.Code.validationConfigurationError.

## See Also

### Getting Birthday Information

var birthday: DateComponents?

A date component for the Gregorian birthday of the contact.

var nonGregorianBirthday: DateComponents?

A date component for the non-Gregorian birthday of the contact.

