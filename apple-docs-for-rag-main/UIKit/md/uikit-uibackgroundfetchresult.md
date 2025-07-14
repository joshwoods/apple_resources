

- UIKit
-  UIBackgroundFetchResult 

Enumeration

# UIBackgroundFetchResult

Constants that indicate the result of a background fetch operation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum UIBackgroundFetchResult
```

## Topics

### Constants

case newData

New data was successfully downloaded.

case noData

There was no new data to download.

case failed

An attempt to download data was made but that attempt failed.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Downloading data in the background

func application(UIApplication, handleEventsForBackgroundURLSession: String, completionHandler: () -> Void)

Tells the delegate that events related to a URL session are waiting to be processed.

