

- TVMLKit JS
- NavigationDocument
-  pushDocument 

Instance Method

# pushDocument

Pushes the specified document onto the stack.

tvOS 9.0+

``` source
void pushDocument(
    in Document document
);
```

## Parameters 

`document`  

The DOM document that is to be added onto the stack.

## Discussion

The document being pushed onto the stack must be a valid parsed DOM object.

## See Also

### Adding Documents to the Stack

insertBeforeDocument

Inserts a new document directly before a document currently on the stack.

replaceDocument

Replaces a document on the stack with a new document.

