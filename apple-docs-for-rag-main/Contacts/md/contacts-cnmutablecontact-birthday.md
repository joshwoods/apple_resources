

- Contacts
- CNMutableContact
-  birthday 

Instance Property

# birthday

A date component for the Gregorian birthday of the contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var birthday: DateComponents? { get set }
```

## Discussion

A Gregorian birthday can be displayed using this property, whose values are the relevant properties of an NSDateComponents object. Day and month are required for this property, and year is optional. Calendar can be `nil` or Gregorian. All other date components are invalid.

## See Also

### Setting Birthday Information

var dates: [CNLabeledValue&lt;NSDateComponents>]

An array containing labeled Gregorian dates.

var nonGregorianBirthday: DateComponents?

A date component for the non-Gregorian birthday of the contact.

