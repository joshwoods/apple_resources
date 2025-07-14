

- TVMLKit JS
- NavigationDocument
-  popToRootDocument 

Instance Method

# popToRootDocument

Removes all documents from the stack except for the bottom-most document, which is the root document.

tvOS 9.0+

``` source
void popToRootDocument();
```

## Discussion

Use this function to quickly return to the root document from any other document in the stack.

## See Also

### Removing Documents from the Stack

clear

Removes all documents currently on the stack.

popDocument

Removes the top most document from the stack.

popToDocument

Removes all of the documents on the stack that are above the passed document.

removeDocument

Removes the specified document from the stack.

