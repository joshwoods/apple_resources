

- TVMLKit JS
- NavigationDocument
-  removeDocument 

Instance Method

# removeDocument

Removes the specified document from the stack.

tvOS 9.0+

``` source
void removeDocument(
    in Document document
);
```

## Parameters 

`document`  

A DOM document created by parsing a TVML file.

## See Also

### Removing Documents from the Stack

clear

Removes all documents currently on the stack.

popDocument

Removes the top most document from the stack.

popToDocument

Removes all of the documents on the stack that are above the passed document.

popToRootDocument

Removes all documents from the stack except for the bottom-most document, which is the root document.

