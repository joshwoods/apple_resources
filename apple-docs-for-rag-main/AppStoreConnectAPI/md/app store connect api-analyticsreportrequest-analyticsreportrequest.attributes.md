

- App Store Connect API
- AnalyticsReportRequest
-  AnalyticsReportRequest.Attributes 

Object

# AnalyticsReportRequest.Attributes

Attributes that describe an analytics report request resource.

App Store Connect API 3.4+

``` source
object AnalyticsReportRequest.Attributes
```

## Properties

`accessType`

`string`

`ONE_TIME_SNAPSHOT`  
A type that provides up-to-the-moment data and goes back as far as is available. It doesn’t generate any new data after the day you request it.

`ONGOING`  
A type that provides current data and is the most typical. It generates daily reports.

Possible Values: `ONE_TIME_SNAPSHOT, ONGOING`

`stoppedDueToInactivity`

`boolean`

Note

Note If you don’t retrieve data for a long time, a report request changes to `stoppedDueToInactivity`. You need to make a new request to resume getting reports.

## See Also

### Objects

object AnalyticsReportRequest.Relationships

