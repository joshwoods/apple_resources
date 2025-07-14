

- App Store Connect API
- AppClipAdvancedExperienceUpdateRequest
- 
  - AppClipAdvancedExperienceUpdateRequest
- AppClipAdvancedExperienceUpdateRequest.Data
- AppClipAdvancedExperienceUpdateRequest.Data.Attributes
- AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place
-  AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.PhoneNumber 

Object

# AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.PhoneNumber

The phone number of a point of interest or business in Apple Maps.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.PhoneNumber
```

## Properties

`intent`

`string`

A string that describes the operational purpose of the phone number; for example `Customer Service` or `Help Desk`

`number`

`string`

The phone number as a string.

`type`

`string`

The resource type.

Possible Values: `FAX, LANDLINE, MOBILE, TOLLFREE`

## See Also

### Objects

object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.DisplayPoint

A point-based representation of a place in Apple Maps.

object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.MainAddress

The main address for a point of interest or business in Apple Maps.

