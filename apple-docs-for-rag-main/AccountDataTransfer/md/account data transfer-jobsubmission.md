

- Account Data Transfer
-  JobSubmission 

Object

# JobSubmission

An object that describes a submission that requests someone’s data.

Account Data Transfer 1.0+

``` source
object JobSubmission
```

## Properties

`mode`

`string`

Whether you want a one-time download, a daily download for 30 days, or a weekly download for 180 days.

Possible Values: `ONE_TIME, DAILY_30, WEEKLY_180`

## See Also

### Request creation

Submit request

Starts preparing someone’s data for download.

object CreatedJob

An object that represents a newly created download request.

Resubmit request

Enqueue the next instance of a recurring request.

object ResubmissionRequest

An object that describes a request to resubmit a recurring download request.

object ResubmissionResponse

An object that represents a resubmitted recurring download request.

