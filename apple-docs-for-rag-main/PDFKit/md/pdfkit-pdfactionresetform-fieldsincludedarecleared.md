

- PDFKit
- PDFActionResetForm
-  fieldsIncludedAreCleared 

Instance Property

# fieldsIncludedAreCleared

Sets whether the fields associated with the reset action are cleared when the action is performed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
var fieldsIncludedAreCleared: Bool { get set }
```

## Parameters 

`include`  

Pass true to clear the fields associated with the action when the reset action is performed. Pass false to exclude from the reset action only the fields associated with the action.

## See Also

### Related Documentation

class PDFActionResetForm

`PDFActionResetForm`, a subclass of `PDFAction`, defines methods for getting and clearing fields in a PDF form.

