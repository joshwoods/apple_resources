

- App Store Connect API
- AppClipAdvancedExperienceCreateRequest
- AppClipAdvancedExperienceCreateRequest.Data
-  AppClipAdvancedExperienceCreateRequest.Data.Attributes 

Object

# AppClipAdvancedExperienceCreateRequest.Data.Attributes

The attributes you set that describe the new Advanced App Clip Experiences resource.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperienceCreateRequest.Data.Attributes
```

## Properties

`action`

AppClipAction

The call-to-action verb that appears on the App Clip card.

`businessCategory`

`string`

The business category of an advanced App Clip experience; for example, `PARKING`

Possible Values: `AUTOMOTIVE, BEAUTY, BIKES, BOOKS, CASINO, EDUCATION, EDUCATION_JAPAN, ENTERTAINMENT, EV_CHARGER, FINANCIAL_USD, FINANCIAL_CNY, FINANCIAL_GBP, FINANCIAL_JPY, FINANCIAL_EUR, FITNESS, FOOD_AND_DRINK, GAS, GROCERY, HEALTH_AND_MEDICAL, HOTEL_AND_TRAVEL, MUSIC, PARKING, PET_SERVICES, PROFESSIONAL_SERVICES, SHOPPING, TICKETING, TRANSIT`

`defaultLanguage`

AppClipAdvancedExperienceLanguage

 (Required) 

The default language for the advanced App Clip experience.

`isPoweredBy`

`boolean`

 (Required) 

A Boolean value that indicates whether the advanced App Clip experience was submitted by a platform provider that serves multiple businesses.

`link`

`uri`

 (Required) 

The invocation URL of the advanced App Clip experience you’re creating.

`place`

AppClipAdvancedExperienceCreateRequest.Data.Attributes.Place

The physical location you associate with the advanced App Clip experience. If you associate an advanced App Clip experience with a place, users can launch your App Clip from from location-based suggestions from Siri Suggestions and the Maps app.

## Topics

### Objects

object AppClipAdvancedExperienceCreateRequest.Data.Attributes.Place

The place information of an advanced App Clip experience you create with this request.

## See Also

### Objects

object AppClipAdvancedExperienceCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

