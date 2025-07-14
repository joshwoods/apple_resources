

- TVMLKit JS
- TVMLKit JS Functions
-  openURL 

Function

# openURL

Opens a deep link into another app.

tvOS 9.0+

``` source
void openURL(
    in String url
);
```

## Parameters 

`url`  

The URL of the app that is to be opened.

## Discussion

Invoking this method with a valid URL launches the handling application.

## See Also

### Manipulating the Document

UUID

Generates a unique UUID.

getActiveDocument

Retrieves the currently active document.

canOpenURL

Determines if a deep-link to another app can be opened.

