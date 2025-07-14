

- Apple Search Ads
-  Apple Search Ads Campaign Management API 2 

Article

# Apple Search Ads Campaign Management API 2

Apple no longer supports this API.

## Overview

Note

As of February 2021, Apple no longer supports the Apple Search Ads Campaign Management API 2. A 301 RESOURCE_MOVED_PERMANENTLY error occurs if you use an API 2 endpoint. API usage requires version 3 or later.

The Apple Search Ads API 2 broadens international support by allowing advertisers to include multiple countries or regions within a single campaign.

API 2 campaigns aren’t compatible with API 3 resources, however, API 2 reports are forward-compatible. Negative keywords and ad groups were decoupled from the campaign object. Negative keywords and targeting keywords were decoupled from ad groups.

The API now represents App Store territories as follows:

`countriesOrRegions`  
For use in the Campaign object.

`countriesOrRegions`  
For use in the ReportingCampaign object.

CountryOrRegion  
For use as a `groupBy` dimension in the ReportingRequest object.

Report field changes are as follows:

| **API 2 report field** | **API 1 report field**    |
|------------------------|---------------------------|
| `installs`             | `conversions`             |
| `latOnInstalls`        | `conversionsLATOn`        |
| `latOffInstalls`       | `conversionsLATOff`       |
| `newDownloads`         | `conversionsNewDownloads` |
| `redownloads`          | `conversionsRedownloads`  |

See ExtendedSpendRow and SpendRow for field descriptions.

API 2 includes the following new features for Creative Sets:

- Creating new Creative Sets and linking to an ad group.

- Reassigning Creative Sets to an ad group.

- Retrieving associated app assets for Creative Sets in campaigns.

- Deleting associated Creative Sets for ad groups.

The following Apple Search Ads Campaign Management API 1 fields are no longer in the corresponding API object and don’t apply to API 2 and later:

`referenceLabel`  
`Campaign object`

`locInvoiceDetails.billingContactName`  
`Campaign object`

`ageCriteria.excluded`  
`TargetingDimensions object`

`genderCriteria.excluded`  
`TargetingDimensions object`

`adminAreaCriteria.excluded`  
`TargetingDimensions object`

`localityCriteria.excluded`  
`TargetingDimensions object`

`deviceClassCriteria.excluded`  
`TargetingDimensions object`

`daypartCriteria.userTime.excluded`  
`TargetingDimensions object`

## See Also

### Changelog

Apple Search Ads Campaign Management API 5

Learn about changes to Apple Search Ads Campaign Management API 5.

Apple Search Ads Campaign Management API 4

Learn about changes to Apple Search Ads Campaign Management API 4.

Apple Search Ads Campaign Management API 3

Apple no longer supports this API.

Apple Search Ads Campaign Management API 1

Apple no longer supports this API.

