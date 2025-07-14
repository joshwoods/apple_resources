

- AppKit
- NSPrinter
-  pageSize(forPaper:) 

Instance Method

# pageSize(forPaper:)

Returns the size of the page for the specified paper type.

macOS

``` source
func pageSize(forPaper paperName: NSPrinter.PaperName) -> NSSize
```

## Parameters 

`paperName`  

Possible values are printer-dependent and are contained in the printer’s PPD file. Typical values are “Letter” and “Legal”.

## Return Value

The size of the page, measured in points in the user coordinate space. The returned size is zero if the specified paper name is not recognized or its entry in the PPD file cannot be parsed.

## See Also

### Getting Page and Printer Information

struct PaperName

The type you use to specify the name of a type of paper.

var languageLevel: Int

The PostScript language level recognized by the printer.

