

- TabularData
- DataFrame
-  joined(\_:on:kind:) 

Instance Method

# joined(\_:on:kind:)

Generates a data frame by joining with another data frame type with a common column that you select by identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func joined(
    _ other: R,
    on columnID: ColumnID,
    kind: JoinKind = .inner
) -> DataFrame where R : DataFrameProtocol, T : Hashable
```

## Parameters 

`other`  

A data frame type that represents the right side of the join.

`columnID`  

A column identifier that exists in both data frame types.

`kind`  

A join operation type.

## Return Value

A new data frame.

## See Also

### Joining two Data Frames

func joined&lt;R>(R, on: String, kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type with a common column you select by name.

func joined&lt;R>(R, on: (left: String, right: String), kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type along the columns that you select by name for both data frame types.

func joined&lt;R, T>(R, on: (left: ColumnID&lt;T>, right: ColumnID&lt;T>), kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type along the columns that you select by identifier for both data frame types.

