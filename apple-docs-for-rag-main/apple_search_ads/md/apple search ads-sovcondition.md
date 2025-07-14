

- Apple Search Ads
-  SovCondition 

Object

# SovCondition

The list of condition objects that allow users to filter a list of records.

Search Ads 4.6+

``` source
object SovCondition
```

## Properties

`field`

`string`

A list of field names to return within each record.

`operator`

`string`

The operator values compare attributes to a list of specified values.

The `IN` operator matches any value in a list of specified values.

Value: `IN`

`values`

`[string]`

A list of matching values.

## Discussion

The `Condition` object functionality is similar to the `WHERE` clause in SQL.

## See Also

### Impression Share Report Request and Response Objects

object CustomReportRequest

The Impression Share report request body.

object CustomReportResponse

A container for Impression Share report metrics.

object CustomReportResponseBody

A container for the Impression Share report response body.

