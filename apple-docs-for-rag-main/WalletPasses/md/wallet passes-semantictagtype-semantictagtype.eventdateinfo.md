

- Wallet Passes
- SemanticTagType
-  SemanticTagType.EventDateInfo 

Object

# SemanticTagType.EventDateInfo

An object that represents a date for an event.

iOS 18.0+iPadOS 6.0+watchOS 2.0+

``` source
object SemanticTagType.EventDateInfo
```

## Properties

`date`

`ISO 8601 date as string`

The date.

`ignoreTimeComponents`

`boolean`

A Boolean value that indicates whether the system ignores the time components of the date.

`timeZone`

`Time zone database identifier as string`

The time zone to display in the date.

`unannounced`

`boolean`

A Boolean value that indicates whether the date of the event is announced.

`undetermined`

`boolean`

A Boolean value that indicates whether the date of the event is determined.

## Discussion

Note

The time zone identifiers come from the IANA time zone database.

## See Also

### Using semantic tag data types

object SemanticTagType.CurrencyAmount

An object that represents an amount of money and type of currency.

object SemanticTagType.Location

An object that represents the coordinates of a location.

object SemanticTagType.PersonNameComponents

An object that represents the parts of a person’s name.

object SemanticTagType.Seat

An object that represents the identification of a seat for a transit journey or an event.

object SemanticTagType.WifiNetwork

An object that contains information required to connect to a WiFi network.

