

- App Store Connect API
- AnalyticsReportRequestCreateRequest
- AnalyticsReportRequestCreateRequest.Data
-  AnalyticsReportRequestCreateRequest.Data.Attributes 

Object

# AnalyticsReportRequestCreateRequest.Data.Attributes

Attributes that describe an analytics report create request resource.

App Store Connect API 3.4+

``` source
object AnalyticsReportRequestCreateRequest.Data.Attributes
```

## Properties

`accessType`

`string`

 (Required) 

The `accessType` `ONGOING` provides current data and is the most typical. It generates reports daily, weekly and monthly. Use `ONE_TIME_SNAPSHOT` to get historical data.

Possible Values: `ONE_TIME_SNAPSHOT, ONGOING`

## See Also

### Objects

object AnalyticsReportRequestCreateRequest.Data.Relationships

