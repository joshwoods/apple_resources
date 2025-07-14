

- TVMLKit JS
- NavigationDocument
-  popToDocument 

Instance Method

# popToDocument

Removes all of the documents on the stack that are above the passed document.

tvOS 9.0+

``` source
void popToDocument(
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

popToRootDocument

Removes all documents from the stack except for the bottom-most document, which is the root document.

removeDocument

Removes the specified document from the stack.

