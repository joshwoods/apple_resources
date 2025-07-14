

- Apple Search Ads
-  EligibilityRecord 

Object

# EligibilityRecord

App eligibility parameters that an API response returns.

Search Ads 4.10+

``` source
object EligibilityRecord
```

## Properties

`adamId`

`int64`

Your unique App Store app identifier.

`countryOrRegion`

`string`

The App Store geoterritories where you’re promoting your app. The value is an ISO 3166-1 alpha-2 country code.

The `EQUALS` and `IN` selector Condition operators are available to use with Find App Eligibility Records.

`deviceClass`

`string`

The eligible devices you can use for targeting. See DeviceClass.

You can use the `EQUALS` and `IN` selector Condition operators with Find App Eligibility Records.

Possible Values: `IPHONE, IPAD`

`minAge`

`int32`

The minimum age you can use to create an ad group. See AgeRange.

Maximum: `65`

`state`

`string`

The system state of the app eligibility review process.

You can use the `EQUALS` and `IN` selector Condition operators with Find App Eligibility Records.

Possible Values: `ELIGIBLE, INELIGIBLE`

`supplySource`

`string`

The ad placements eligible for a campaign.

You can use the `EQUALS` and `IN` selector Condition operators with Find App Eligibility Records.

See SupplySource.

Possible Values: `APPSTORE_SEARCH_RESULTS, APPSTORE_SEARCH_TAB, APPSTORE_PRODUCT_PAGES_BROWSE, APPSTORE_TODAY_TAB`

## See Also

### App Eligibility Request and Response Objects

object EligibilityRecordListResponse

The response details to an app eligibility request.

