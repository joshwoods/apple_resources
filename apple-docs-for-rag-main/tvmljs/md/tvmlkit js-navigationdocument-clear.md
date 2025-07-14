

- TVMLKit JS
- NavigationDocument
-  clear 

Instance Method

# clear

Removes all documents currently on the stack.

tvOS 9.0+

``` source
void clear();
```

## Discussion

No animations are performed when this function is called. All documents currently on the stack are immediately removed.

## See Also

### Removing Documents from the Stack

popDocument

Removes the top most document from the stack.

popToDocument

Removes all of the documents on the stack that are above the passed document.

popToRootDocument

Removes all documents from the stack except for the bottom-most document, which is the root document.

removeDocument

Removes the specified document from the stack.

