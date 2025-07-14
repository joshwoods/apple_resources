

- Core Motion
- CMSensorRecorder
-  accelerometerData(from:to:) 

Instance Method

# accelerometerData(from:to:)

Retrieves the accelerometer data collected between the specified dates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func accelerometerData(
    from fromDate: Date,
    to toDate: Date
) -> CMSensorDataList?
```

## Parameters 

`fromDate`  

The starting date (inclusive) from which to retrieve data. Entries occurring before this date are excluded from the results.

`toDate`  

The end date (inclusive) at which to stop retrieving data. Entries occurring after this date are excluded from the results. The difference in time between the `fromDate` and this parameter must be 12 hours or less.

## Return Value

An object to use for enumerating over the accelerometer data.

## Discussion

Use this method to fetch accelerometer data entries in the specified date range. When fetching entries for a date range, the recorder returns only the data entries it has. If there were gaps in the recording, no data entries are returned for those gaps. Recorded accelerometer data is kept for a maximum of three days. There may be a delay of up to three minutes before new samples are available for retrieval.

