

- Screen Time
- STWebHistory
-  deleteHistory(during:) 

Instance Method

# deleteHistory(during:)

Deletes web history that occurred during the date interval you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
func deleteHistory(during interval: DateInterval)
```

## Parameters 

`interval`  

The date interval of web history you want to delete.

## See Also

### Instance methods

func deleteAllHistory()

Deletes all web history associated with the bundle identifier you specified during initialization.

func deleteHistory(for: URL)

Deletes all the web history for the URL you specify.

