

- PDFKit
- PDFActionResetForm
-  fields 

Instance Property

# fields

Returns an array of fields associated with the reset action.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
var fields: [String]? { get set }
```

## Return Value

An array of `NSString` objects that corresponds to the `fieldNames` property of widget annotations (such as PDFAnnotationButtonWidget) on the PDF page. This method can return `NULL`.

## See Also

### Related Documentation

class PDFActionResetForm

`PDFActionResetForm`, a subclass of `PDFAction`, defines methods for getting and clearing fields in a PDF form.

