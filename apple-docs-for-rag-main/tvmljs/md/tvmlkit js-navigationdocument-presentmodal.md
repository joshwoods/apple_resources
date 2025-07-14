

- TVMLKit JS
- NavigationDocument
-  presentModal 

Instance Method

# presentModal

Displays the passed document on top of the current document.

tvOS 9.0+

``` source
void presentModal(
    in Document document
);
```

## Parameters 

`document`  

A DOM document created by parsing a TVML file.

## Discussion

The passed document is presented on top of the current document. The current document is blurred and is used as the background for the modal document.

## See Also

### Overlaying Document

dismissModal

Dismisses the document displayed in modal view.

