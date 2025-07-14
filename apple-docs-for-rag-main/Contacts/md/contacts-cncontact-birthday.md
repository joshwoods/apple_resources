

- Contacts
- CNContact
-  birthday 

Instance Property

# birthday

A date component for the Gregorian birthday of the contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var birthday: DateComponents? { get }
```

## Discussion

Birthdays are represented by this property, whose values are the relevant properties of an NSDateComponents object. Day and month components are required for this property, and year is optional. The calendar component can be `nil` or gregorian. All other date components are invalid and including them results in an NSError object that includes the key paths of the invalid components and the error code CNError.Code.validationConfigurationError.

## See Also

### Getting Birthday Information

var nonGregorianBirthday: DateComponents?

A date component for the non-Gregorian birthday of the contact.

var dates: [CNLabeledValue&lt;NSDateComponents>]

An array containing labeled Gregorian dates.

