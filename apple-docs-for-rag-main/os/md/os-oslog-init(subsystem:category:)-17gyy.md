

- os
- OSLog
-  init(subsystem:category:) 

Initializer

# init(subsystem:category:)

Creates a log using the specified subsystem and category.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
convenience init(
    subsystem: String,
    category: String
)
```

## Parameters 

`subsystem`  

An identifier string, in reverse DNS notation, that represents the app subsystem that’s logging information, such as `com.your_company.your_subsystem_name`. The logging system uses this information to categorize and filter related log messages, and to group related logging settings.

`category`  

A category within the specified subsystem. The system uses this value to categorize and filter related log messages, and to group related logging settings within the subsystem. A category’s logging settings override those of the containing subsystem.

## Return Value

A custom log object that you can pass to other logging functions to perform logging and to determine whether a specific level of logging is in an enabled state.

## See Also

### Creating a Log

convenience init(subsystem: String, category: OSLog.Category)

Creates a log using the specified subsystem and system-defined category.

struct Category

System-defined categories that identify well-known parts of your app.

