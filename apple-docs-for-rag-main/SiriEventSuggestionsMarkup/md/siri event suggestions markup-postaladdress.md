

- Siri Event Suggestions Markup
-  PostalAddress 

Object

# PostalAddress

A specific geographic location.

Siri Event Suggestions Markup 1.0+

``` source
object PostalAddress
```

## Properties

`@type`

`string`

 (Required) 

Value: `PostalAddress`

`addressCountry`

`string`

 (Required) 

The country.

`addressLocality`

`string`

 (Required) 

The city or town.

`addressRegion`

`string`

The region containing the locality.

`postalCode`

`string`

The postal code.

`streetAddress`

`string`

 (Required) 

The street name and number.

## Discussion

Prefer a physical address, not an administrative mailing address, to help Siri and Maps provide relevant information to the user.

## See Also

### Common Reservation Data

object Person

A passenger, diner, lodging guest, or event attendee.

object Ticket

Details about a ticket for transportation or an event.

object Seat

The specific location reserved for the passenger.

object Organization

A business, transportation provider, or event organizer.

object Place

A business, transportation hub, or event venue.

