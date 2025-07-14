

- SwiftUI
- TableRow
-  init(\_:) 

Initializer

# init(\_:)

Creates a table row for the given value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
init(_ value: Value)
```

## Parameters 

`value`  

The value of the row.

## Discussion

The table provides the value of a row to each column of a table, which produces the cells for each row in the column.

The following example creates a row for one instance of the `Person` type. The table delivers this value to its columns, which displays different fields of `Person`.

```
 TableRow(Person(givenName: "Tom", familyName: "Clark"))
```

