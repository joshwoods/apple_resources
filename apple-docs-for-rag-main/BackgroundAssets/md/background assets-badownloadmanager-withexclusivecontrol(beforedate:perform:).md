

- Background Assets
- BADownloadManager
-  withExclusiveControl(beforeDate:perform:) 

Instance Method

# withExclusiveControl(beforeDate:perform:)

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
func withExclusiveControl(
    beforeDate date: Date,
    perform performHandler: @escaping (Bool, (any Error)?) -> Void
)
```

## See Also

### Synchronizing manager access

func withExclusiveControl((Bool, (any Error)?) -> Void)

Attempts to acquire immediate, exclusive access to the download manager.

