

- Contacts
- CNMutableContact
-  nonGregorianBirthday 

Instance Property

# nonGregorianBirthday

A date component for the non-Gregorian birthday of the contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var nonGregorianBirthday: DateComponents? { get set }
```

## Discussion

A non-Gregorian birthday such as Lunisolar birthdays can be displayed using this property, whose values are the relevant properties of an NSDateComponents object. Day and month are required; year and isLeapMonth are optional. The calendar property is also required and must be non-Gregorian. Some supported calendars are Buddhist, Chinese, or Islamic. All other date components are invalid.

## See Also

### Setting Birthday Information

var dates: [CNLabeledValue&lt;NSDateComponents>]

An array containing labeled Gregorian dates.

var birthday: DateComponents?

A date component for the Gregorian birthday of the contact.

