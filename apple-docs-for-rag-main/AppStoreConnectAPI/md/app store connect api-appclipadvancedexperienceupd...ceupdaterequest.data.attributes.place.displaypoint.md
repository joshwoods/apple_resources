

- App Store Connect API
- AppClipAdvancedExperienceUpdateRequest
- 
  - AppClipAdvancedExperienceUpdateRequest
- AppClipAdvancedExperienceUpdateRequest.Data
- AppClipAdvancedExperienceUpdateRequest.Data.Attributes
- AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place
-  AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.DisplayPoint 

Object

# AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.DisplayPoint

A point-based representation of a place in Apple Maps.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.DisplayPoint
```

## Properties

`coordinates`

AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.DisplayPoint.Coordinates

The GPS coordinates of a place in Apple Maps you associate with the Advanced App Clip experience.

`source`

`string`

A string that describes the means by which you captured the data for a display point.

Possible Values: `CALCULATED, MANUALLY_PLACED`

## Topics

### Objects

object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.DisplayPoint.Coordinates

The coordinates for a point of interest or business in Apple Maps.

## See Also

### Objects

object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.MainAddress

The main address for a point of interest or business in Apple Maps.

object AppClipAdvancedExperienceUpdateRequest.Data.Attributes.Place.PhoneNumber

The phone number of a point of interest or business in Apple Maps.

