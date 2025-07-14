

- Foundation
- ISO8601DateFormatter
-  init() 

Initializer

# init()

Initializes an ISO 8601 date formatter with default format, time zone, and options.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init()
```

## Discussion

By default, a formatter is initialized to use the GMT time zone, the RFC 3339 standard format (`"yyyy-MM-dd'T'HH:mm:ssZZZZZ"`), and the following options: withInternetDateTime, withDashSeparatorInDate, withColonSeparatorInTime, and withTimeZone.

This is the designated initializer.

