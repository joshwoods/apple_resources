

- TVMLKit JS
- NavigationDocument
-  replaceDocument 

Instance Method

# replaceDocument

Replaces a document on the stack with a new document.

tvOS 9.0+

``` source
void replaceDocument(
    in Document document, 
    in Document oldDocument
);
```

## Parameters 

`document`  

The DOM document that is to be added onto the stack.

`oldDocument`  

The DOM document that is being replaced.

## Discussion

This function searches the stack for the first instance of the document to be replaced and replaces it with the new document.

## See Also

### Adding Documents to the Stack

insertBeforeDocument

Inserts a new document directly before a document currently on the stack.

pushDocument

Pushes the specified document onto the stack.

