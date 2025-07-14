

- Contacts
- CNContact
-  nonGregorianBirthday 

Instance Property

# nonGregorianBirthday

A date component for the non-Gregorian birthday of the contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var nonGregorianBirthday: DateComponents? { get }
```

## Discussion

Non-Gregorian birthdays can be displayed using this property, which has values that are the relevant properties of an NSDateComponents object. Day and month components are required; year and leap month are optional. The calendar component is also required and must be an NSCalendar object with an identifier other than gregorian. For example, some supported calendars are Chinese, Hebrew, or Islamic. All other date components are invalid and including them results in an NSError object that includes the key paths of the invalid components and the error code CNError.Code.validationConfigurationError.

## See Also

### Getting Birthday Information

var birthday: DateComponents?

A date component for the Gregorian birthday of the contact.

var dates: [CNLabeledValue&lt;NSDateComponents>]

An array containing labeled Gregorian dates.

