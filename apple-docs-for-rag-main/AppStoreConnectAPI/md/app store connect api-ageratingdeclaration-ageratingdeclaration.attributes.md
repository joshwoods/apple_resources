

- App Store Connect API
- AgeRatingDeclaration
-  AgeRatingDeclaration.Attributes 

Object

# AgeRatingDeclaration.Attributes

Attributes that describe an Age Rating Declarations resource.

App Store Connect API 1.2+

``` source
object AgeRatingDeclaration.Attributes
```

## Properties

`alcoholTobaccoOrDrugUseOrReferences`

`string`

Declaration for alcohol, tobacco, or drug use.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`gamblingAndContests`

`boolean`

Deprecated 

Declaration for gambling or contests, as a Boolean value.

`kidsAgeBand`

KidsAgeBand

Declaration for the Kids Age Band value.

`medicalOrTreatmentInformation`

`string`

Declaration for medical or treatment-focused content.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`profanityOrCrudeHumor`

`string`

Declaration for profanity or crude humor.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`sexualContentOrNudity`

`string`

Declaration for sexual content or nudity.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`unrestrictedWebAccess`

`boolean`

Declaration for unrestricted web access, such as with an embedded browser, provided as a Boolean value.

`gamblingSimulated`

`string`

Declaration for simulated gambling.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`horrorOrFearThemes`

`string`

Declaration for horror or fear themed content.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`matureOrSuggestiveThemes`

`string`

Declaration for mature or suggestive themes.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`sexualContentGraphicAndNudity`

`string`

Declaration for graphic sexual content and nudity.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`violenceCartoonOrFantasy`

`string`

Declaration for cartoon or fantasy violence.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`violenceRealistic`

`string`

Declaration for realistic violence.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`violenceRealisticProlongedGraphicOrSadistic`

`string`

Declaration for prolonged realistic or sadistic violence.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`contests`

`string`

Declaration for contests.

Possible Values: `NONE, INFREQUENT_OR_MILD, FREQUENT_OR_INTENSE`

`gambling`

`boolean`

Declaration for gambling, provided as a Boolean value.

`seventeenPlus`

`boolean`

Deprecated 

Declaration for a 17+ rating, provided as a Boolean value.

`ageRatingOverride`

`string`

Possible Values: `NONE, SEVENTEEN_PLUS, UNRATED`

`koreaAgeRatingOverride`

`string`

Possible Values: `NONE, FIFTEEN_PLUS, NINETEEN_PLUS`

`lootBox`

`boolean`

## Mentioned in 

App Store Connect API 1.3 release notes

