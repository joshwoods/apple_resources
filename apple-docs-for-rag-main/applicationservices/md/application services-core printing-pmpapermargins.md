

- Application Services
- Core Printing
-  PMPaperMargins 

Type Alias

# PMPaperMargins

A data structure that specifies the unprintable area of a paper object.

macOS 10.3+

``` source
typealias PMPaperMargins = PMRect
```

## Discussion

Your application specifies paper margins when calling the function PMPaperCreateCustom(_:_:_:_:_:_:_:) to create a custom paper type. You can obtain a paper’s margins with the function PMPaperGetMargins(_:_:).

