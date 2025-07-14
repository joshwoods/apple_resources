

- ContactProvider
- ContactItemContentObserver
-  didFinishEnumeratingContent(upTo:) 

Instance Method

# didFinishEnumeratingContent(upTo:)

Finishes the content enumeration to the observer.

iOS 18.0+iPadOS 18.0+

``` source
func didFinishEnumeratingContent(upTo generationMarker: Data)
```

**Required**

## Parameters 

`generationMarker`  

A value specific to your data source identifying the database generation whose content has been enumerated.

## Discussion

Call this when there are no more items to enumerate. Any future item enumerations after this are change enumerations. The first change enumeration begins from `generationMarker`, which syncs changes made after the content enumeration began. Calling this method saves the current page of items to the system Contacts database.

## See Also

### Ending enumeration

func didFinishEnumeratingPage(upTo: ContactItemPage)

Marks a page of items as completed.

**Required**

struct ContactItemPage

A fixed offset into enumerating all contact items.

func didFinishEnumeratingContentWithError(any Error)

Finishes the content enumeration with an error, indicating failure, to the observer.

**Required**

