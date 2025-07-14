

- TVMLKit JS
- NavigationDocument
-  insertBeforeDocument 

Instance Method

# insertBeforeDocument

Inserts a new document directly before a document currently on the stack.

tvOS 9.0+

``` source
void insertBeforeDocument(
    in Document document, 
    in optional Document beforeDocument
);
```

## Parameters 

`document`  

The DOM document that is to be added onto the stack.

`beforeDocument`  

A DOM document currently on the stack. The new document is placed on the stack directly after this document.

## Discussion

This function searches the stack for the first instance of the document contained in the `beforeDocument` parameter and inserts the document contained in the `document` parameter on top of it.

## See Also

### Adding Documents to the Stack

pushDocument

Pushes the specified document onto the stack.

replaceDocument

Replaces a document on the stack with a new document.

