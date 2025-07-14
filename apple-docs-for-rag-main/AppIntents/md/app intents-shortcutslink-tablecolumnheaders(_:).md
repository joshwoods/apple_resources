

- App Intents
- ShortcutsLink
-  tableColumnHeaders(\_:) 

Instance Method

# tableColumnHeaders(\_:)

Controls the visibility of a `Table`’s column header views.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func tableColumnHeaders(_ visibility: Visibility) -> some View
```

## Parameters 

`visibility`  

A value of `visible` will show table columns, `hidden` will remove them, and `automatic` will defer to default behavior.

## Discussion

By default, `Table` will display a global header view with the labels of each table column. This area is also where users can sort, resize, and rearrange the columns. For simple cases that don’t require those features, this header can be hidden.

This will not affect the header of any `Section`s in a table.

```
Table(article.authors) {
    TableColumn("Name", value: \.name)
    TableColumn("Title", value: \.title)
}
.tableColumnHeaders(.hidden)
```

