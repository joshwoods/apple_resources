

- os
- OSLog
-  init(subsystem:category:) 

Initializer

# init(subsystem:category:)

Creates a log using the specified subsystem and system-defined category.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOSwatchOS 5.0+

``` source
convenience init(
    subsystem: String,
    category: OSLog.Category
)
```

## Parameters 

`subsystem`  

An identifier string, in reverse DNS notation, that represents the subsystem that’s performing logging, such as `com.your_company.your_subsystem_name`. The logging system uses this information to categorize and filter related log messages.

`category`  

A system-defined category within the specified subsystem. The system uses this value to categorize and filter related log messages. A category’s logging settings override those of the containing subsystem.

## Return Value

A custom log object that you can pass to other logging functions to perform logging and to determine whether a specific level of logging is in an enabled state.

## See Also

### Creating a Log

convenience init(subsystem: String, category: String)

Creates a log using the specified subsystem and category.

struct Category

System-defined categories that identify well-known parts of your app.

