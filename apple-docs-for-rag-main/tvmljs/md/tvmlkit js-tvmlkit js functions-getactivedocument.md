

- TVMLKit JS
- TVMLKit JS Functions
-  getActiveDocument 

Function

# getActiveDocument

Retrieves the currently active document.

tvOS 9.0+

``` source
Document getActiveDocument();
```

## Return Value

The currently active document.

## Discussion

The currently active document is the document that the user is interacting with. It can be the document on top of the navigation stack or a modally presented document. If the a menu bar document is the top most document, this function returns the document that is selected in the Menu Bar.

## See Also

### Manipulating the Document

UUID

Generates a unique UUID.

canOpenURL

Determines if a deep-link to another app can be opened.

openURL

Opens a deep link into another app.

