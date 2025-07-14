

- ClockKit
- CLKComplicationServer
-  reloadComplicationDescriptors() Deprecated

Instance Method

# reloadComplicationDescriptors()

Reloads the complication descriptors from the complication data source.

watchOS 7.0–9.0Deprecated

``` source
func reloadComplicationDescriptors()
```

## Mentioned in 

Declaring complications for your app

## Discussion

Call this method to reload the complication descriptors from your data source. ClockKit then calls your data source’s getComplicationDescriptors(handler:) method to update the list of available complications.

If your data source removes a complication that’s already present on a watch face, ClockKit continues to display the complication and to request new timeline entries for that complication. However, the user won’t be able to add the complication to new watch faces.

