

- Foundation
- NSQuitCommand
-  saveOptions 

Instance Property

# saveOptions

Returns a constant indicating how to deal with closing any modified documents.

Mac Catalyst 13.0+macOS 10.0+

``` source
var saveOptions: NSSaveOptions { get }
```

## Return Value

A constant indicating how to deal with closing any modified documents.

## Discussion

The default value returned is `NSSaveOptionsAsk`. See “Constants” in NSCloseCommand for a list of possible return values.

## See Also

### Related Documentation

Cocoa Scripting Guide

