

- AppKit
- NSPrinter
-  languageLevel 

Instance Property

# languageLevel

The PostScript language level recognized by the printer.

macOS

``` source
var languageLevel: Int { get }
```

## Return Value

The PostScript language level. The value is 0 if the receiver is not a PostScript printer.

## See Also

### Getting Page and Printer Information

func pageSize(forPaper: NSPrinter.PaperName) -> NSSize

Returns the size of the page for the specified paper type.

struct PaperName

The type you use to specify the name of a type of paper.

