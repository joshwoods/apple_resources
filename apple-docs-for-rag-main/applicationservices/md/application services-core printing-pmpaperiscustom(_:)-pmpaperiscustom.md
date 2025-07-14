

- Application Services
- Core Printing
-  PMPaperIsCustom(\_:) 

Function

# PMPaperIsCustom(\_:)

Returns a Boolean value indicating whether a specified paper is a custom paper.

macOS 10.5+

``` source
func PMPaperIsCustom(_ paper: PMPaper) -> Bool
```

## Parameters 

`paper`  

The paper you’re querying to determine whether it’s a custom paper.

## Return Value

If `true`, the specified paper is a custom paper; otherwise, `false`.

## Discussion

You can create a custom paper with the function PMPaperCreateCustom(_:_:_:_:_:_:_:).

## See Also

### Creating and Using Paper Objects

func PMPaperCreateCustom(PMPrinter?, CFString?, CFString?, Double, Double, UnsafePointer&lt;PMPaperMargins>, UnsafeMutablePointer&lt;PMPaper?>) -> OSStatus

Creates a custom paper object.

