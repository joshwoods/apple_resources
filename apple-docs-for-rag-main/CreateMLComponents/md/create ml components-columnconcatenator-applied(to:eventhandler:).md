

- Create ML Components
- ColumnConcatenator
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Combines every numerical column in a data frame into to a shaped array for each row.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: DataFrame,
    eventHandler: EventHandler? = nil
) throws -> DataFrame
```

