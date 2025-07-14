

- App Store Connect API
- AppClipAdvancedExperienceUpdateRequest
- AppClipAdvancedExperienceUpdateRequest.Data
- AppClipAdvancedExperienceUpdateRequest.Data.Attributes
-  AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place 

Object

# AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place

The place information of an advanced App Clip experience you create with this request.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place
```

## Properties

`categories`

`[string]`

A list of categories for a place in Apple Maps you associate with the Advanced App Clip experience.

`displayPoint`

AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.DisplayPoint

Coordinates of a place in Apple Maps you associate with an advanced App Clip experience.

`homePage`

`string`

The optional website URL for a place.

`mainAddress`

AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.MainAddress

The main address of a place in Apple Maps. This value is required if you don’t provide coordinates for a place.

`mapAction`

`string`

A string that describes the intent behind an App Clip invocation from location-based suggestions from Siri Suggestions and the Maps app.

Possible Values: `BUY_TICKETS, VIEW_AVAILABILITY, VIEW_PRICING, HOTEL_BOOK_ROOM, PARKING_RESERVE_PARKING, RESTAURANT_JOIN_WAITLIST, RESTAURANT_ORDER_DELIVERY, RESTAURANT_ORDER_FOOD, RESTAURANT_ORDER_TAKEOUT, RESTAURANT_RESERVATION, SCHEDULE_APPOINTMENT, RESTAURANT_VIEW_MENU, THEATER_NOW_PLAYING`

`names`

`[string]`

An array of names as strings for a place in Apple Maps.

`phoneNumber`

AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.PhoneNumber

The phone number that’s associated with a place in Apple Maps as a string.

`placeId`

`string`

An opaque ID that uniquely identifies a place. If you previously created a place in Apple Maps for the place you associate with your advanced App Clip experience, use its ID instead of creating a new ID.

`relationship`

`string`

A navigational link to related data and included resource types and IDs.

Possible Values: `OWNER, AUTHORIZED, OTHER`

## Topics

### Objects

object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.DisplayPoint

A point-based representation of a place in Apple Maps.

object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.MainAddress

The main address for a point of interest or business in Apple Maps.

object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.PhoneNumber

The phone number of a point of interest or business in Apple Maps.

