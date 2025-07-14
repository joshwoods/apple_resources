

- App Store Connect API
- AppClipAdvancedExperience
- 
  - AppClipAdvancedExperience
- AppClipAdvancedExperience.Attributes
- AppClipAdvancedExperience.Attributes.Place
- AppClipAdvancedExperience.Attributes.Place.MainAddress
-  AppClipAdvancedExperience.Attributes.Place.MainAddress.StructuredAddress 

Object

# AppClipAdvancedExperience.Attributes.Place.MainAddress.StructuredAddress

The structured address information for a point of interest or business in Apple Maps.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperience.Attributes.Place.MainAddress.StructuredAddress
```

## Properties

`countryCode`

`string`

The country code of a place in Apple Maps you associate with the Advanced App Clip experience.

`floor`

`string`

The identifier of a floor in a building.

`locality`

`string`

The official locality component of a postal address; for example, a city or town.

`neighborhood`

`string`

The sub-locality component of a postal address; for example, a borough, county, or municipality.

`postalCode`

`string`

The mail sorting code associated with a postal address.

`stateProvince`

`string`

The province component of a postal address; for example, a state or territory.

`streetAddress`

`[string]`

The officially recognized address used by a postal delivery address. It includes — when applicable — a street name, street suffix, building, house, or suite identifiers.

