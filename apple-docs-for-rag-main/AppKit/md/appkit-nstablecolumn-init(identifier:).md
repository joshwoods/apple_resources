

- AppKit
- NSTableColumn
-  init(identifier:) 

Initializer

# init(identifier:)

Initializes a newly created table column with a string identifier.

macOS

``` source
@MainActor
init(identifier: NSUserInterfaceItemIdentifier)
```

## Parameters 

`identifier`  

The string identifier for the column.

## Return Value

An initialized table column instance with an NSTextFieldCell instance as its default cell.

## Discussion

You can set the table column title using the title property.

This method is the designated initializer for the `NSTableColumn` class.

## See Also

### Related Documentation

Table View Programming Guide for Mac

var identifier: NSUserInterfaceItemIdentifier

The identifier string for the table column.

