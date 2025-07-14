

- App Store Connect API
-  Download Sales and Trends Reports 

Web Service Endpoint

# Download Sales and Trends Reports

Download sales and trends reports filtered by your specified criteria.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/salesReports
```

## Query Parameters

`filter[frequency]`

`[string]`

 (Required) 

Frequency of the report to download. For a list of values, see Allowed values based on sales report type table below.

Possible Values: `DAILY, WEEKLY, MONTHLY, YEARLY`

`filter[reportDate]`

`[string]`

The report date to download. Specify the date in the `YYYY-MM-DD` format for all report frequencies except `DAILY`, which doesn’t require a date. For more information, see report availability and storage.

`filter[reportSubType]`

`[string]`

 (Required) 

The report sub type to download. For a list of values, see Allowed values based on sales report type table below.

Possible Values: `SUMMARY, DETAILED, SUMMARY_INSTALL_TYPE, SUMMARY_TERRITORY, SUMMARY_CHANNEL`

`filter[reportType]`

`[string]`

 (Required) 

The report to download. For more details on each report type see Download and view reports.

Possible Values: `SALES, PRE_ORDER, NEWSSTAND, SUBSCRIPTION, SUBSCRIPTION_EVENT, SUBSCRIBER, SUBSCRIPTION_OFFER_CODE_REDEMPTION, INSTALLS, FIRST_ANNUAL, WIN_BACK_ELIGIBILITY`

`filter[vendorNumber]`

`[string]`

 (Required) 

You can find your vendor number in View payments and proceeds.

`filter[version]`

`[string]`

The version of the report. For a list of values, see Allowed values based on sales report type table below.

## Response Codes

` 200 ``OK`

gzip

`OK`

The request completed successfully.

Content-Type: application/a-gzip

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

## Mentioned in 

App Store Connect API 3.6 release notes

App Store Connect API 3.2 release notes

App Store Connect API 3.4 release notes

App Store Connect API 3.7 release notes

App Store Connect API 1.8 release notes

## Discussion

### Allowed values based on sales report type

Each sales report type has specific valid values for `reportType`, `reportSubType`, `frequency`, and `version`. If you use other types, it results in an error. For more details on each report type, see Download and view reports.

Note

Version 1_2 of the Subscription, Subscription Event, and Subscriber reports in Sales and Trends is no longer available for download.

| `reportType` | `reportSubType` | `frequency` | `version` |
|----|----|----|----|
| FIRST_ANNUAL | DETAILED | DAILY | 1_0 |
| FIRST_ANNUAL | SUMMARY | YEARLY | 1_0 |
| INSTALLS | SUMMARY_CHANNEL | YEARLY | 1_0, 1_1 |
| INSTALLS | SUMMARY_INSTALL_TYPE | YEARLY | 1_0, 1_1 |
| INSTALLS | SUMMARY | MONTHLY | 1_2 |
| INSTALLS | SUMMARY_TERRITORY | YEARLY | 1_0, 1_1 |
| INSTALLS | DETAILED | MONTHLY | 1_2 |
| INSTALLS | DETAILED | YEARLY | 1_0, 1_1 |
| NEWSSTAND | DETAILED | DAILY, WEEKLY | 1_0 |
| PRE_ORDER | SUMMARY | DAILY, WEEKLY, MONTHLY, YEARLY | 1_0 |
| SALES | SUMMARY | DAILY, WEEKLY, MONTHLY, YEARLY | 1_0 |
| SUBSCRIBER | DETAILED | DAILY | 1_3 |
| SUBSCRIPTION | SUMMARY | DAILY | 1_3 |
| SUBSCRIPTION_EVENT | SUMMARY | DAILY | 1_3 |
| SUBSCRIPTION_OFFER_CODE_REDEMPTION | SUMMARY | DAILY | 1_0 |
| WIN_BACK_ELIGIBILITY | SUMMARY | DAILY | 1_0 |

## See Also

### Downloading Reports

Download Finance Reports

Download finance reports filtered by your specified criteria.

