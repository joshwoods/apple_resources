

- Screen Time
- STWebHistory
-  deleteHistory(for:) 

Instance Method

# deleteHistory(for:)

Deletes all the web history for the URL you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
func deleteHistory(for url: URL)
```

## Parameters 

`url`  

The URL associated with the web history to delete.

## Discussion

The framework references the entire URL to determine which web-usage data to delete.

## See Also

### Instance methods

func deleteAllHistory()

Deletes all web history associated with the bundle identifier you specified during initialization.

func deleteHistory(during: DateInterval)

Deletes web history that occurred during the date interval you specify.

