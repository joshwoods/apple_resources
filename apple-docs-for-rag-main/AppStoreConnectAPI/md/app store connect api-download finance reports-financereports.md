

- App Store Connect API
-  Download Finance Reports 

Web Service Endpoint

# Download Finance Reports

Download finance reports filtered by your specified criteria.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/financeReports
```

## Query Parameters

`filter[regionCode]`

`[string]`

 (Required) 

You can download consolidated or separate financial reports per territory. For a complete list of possible values, see Financial report regions and currencies.

`filter[reportDate]`

`[string]`

 (Required) 

The fiscal month of the report you wish to download based on the Apple Fiscal Calendar. The fiscal month is specified in the `YYYY-MM` format.

`filter[reportType]`

`[string]`

 (Required) 

This value is always `FINANCIAL`.

Possible Values: `FINANCIAL, FINANCE_DETAIL`

`filter[vendorNumber]`

`[string]`

 (Required) 

You can find your vendor number in View payments and proceeds.

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

Downloading Analytics Reports

## Discussion

For more information see Download financial reports.

## See Also

### Downloading Reports

Download Sales and Trends Reports

Download sales and trends reports filtered by your specified criteria.

