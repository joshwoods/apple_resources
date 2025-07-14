

- Create ML
- MLDataTable
-  map(\_:) 

Instance Method

# map(\_:)

Creates a new column by applying a given thread-safe transform to every row in the data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func map(_ lazyTransform: @escaping (MLDataTable.Row) -> T) -> MLDataColumn where T : MLDataValueConvertible
```

## Parameters 

`lazyTransform`  

A thread-safe row transformation function.

The implementation of your transform must accept a row from the data table and return a type that conforms to MLDataValueConvertible.

## Return Value

A new MLDataColumn.

## Discussion

Use this method to create a new column derived from the existing data in the table. The closure you pass evaluates lazily only when the transformed values are needed for a subsequent operation. Your implementation should accept a data table row and must be thread-safe because the framework may invoke the closure concurrently on unspecified threads.

For example, to perform the column derivation operation shown above, begin by creating a table of data.

```
let data: [String: MLDataValueConvertible] = [
    "Day": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
    "Temperature": [91.3, 85.8, 79.5, 83.4, 72.2]
]

var table = try MLDataTable(dictionary: data)
```

After creating the table, use map(_:) to create a new column of data from the original data. The example closure implementation below is stateless and safe to invoke concurrently on any thread, so no synchronization is necessary.

```
let derivedColumn = table.map { row -> String in
    guard let day = row["Day"]?.stringValue,
          let temperature = row["Temperature"]?.doubleValue else {
            fatalError("Missing or invalid columns in row.")
    }
    return String(format: "%@ %.1fº", day, temperature)
}
```

Then use addColumn(_:named:) to add the derived column to a table.

```
table.addColumn(derivedColumn, named: "Description")
```

## See Also

### Related Documentation

Preventing Timing Problems When Using Closures

Understand how different API calls to your closures can affect your app.

func map&lt;T>((MLDataTable.Row) -> T?) -> MLDataColumn&lt;T>

Creates a new column, potentially with missing values, by applying a given thread-safe transform to every row in the data table.

### Transforming rows to generate a data column

func map&lt;T>((MLDataTable.Row) -> T?) -> MLDataColumn&lt;T>

Creates a new column, potentially with missing values, by applying a given thread-safe transform to every row in the data table.

