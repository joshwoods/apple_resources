

- ContactProvider
- ContactItemContentObserver
-  didFinishEnumeratingPage(upTo:) 

Instance Method

# didFinishEnumeratingPage(upTo:)

Marks a page of items as completed.

iOS 18.0+iPadOS 18.0+

``` source
func didFinishEnumeratingPage(upTo nextPage: ContactItemPage)
```

**Required**

## Parameters 

`nextPage`  

The ContactItemPage where the next content enumeration can continue.

## Discussion

Call this method only if there are more items to enumerate after this page. An interrupted content enumeration can resume in the future, continuing from this page. Calling this method saves the current page of items to the system Contacts database.

## See Also

### Ending enumeration

func didFinishEnumeratingContent(upTo: Data)

Finishes the content enumeration to the observer.

**Required**

struct ContactItemPage

A fixed offset into enumerating all contact items.

func didFinishEnumeratingContentWithError(any Error)

Finishes the content enumeration with an error, indicating failure, to the observer.

**Required**

