

- ContactProvider
- ContactItemEnumerator
-  enumerateContent(in:for:) 

Instance Method

# enumerateContent(in:for:)

Enumerates all items, batched in pages.

iOS 18.0+iPadOS 18.0+

``` source
func enumerateContent(
    in page: ContactItemPage,
    for observer: any ContactItemContentObserver
) async
```

**Required**

## Parameters 

`page`  

The page to enumerate items from.

`observer`  

The system observer that receives the content items and enumeration state.

## Discussion

The system calls `enumerateContent(in:for:)` for each page of items to enumerate. Your implementation calls didFinishEnumeratingPage(upTo:) after enumerating each page, excluding the last page. After enumerating the last page, your implementation calls didFinishEnumeratingContent(upTo:).

Your implementation can enumerate items in any order, but the order must be deterministic and resumable. The system starts a new content enumeration with initialPage.

During content enumeration, every ContactItemPage except initialPage must use the same generationMarker, which represents the state of the content at a specific point in time. Changes made during the content enumeration can sync later with a change enumeration.

## See Also

### Enumerating contact items

struct ContactItemPage

A fixed offset into enumerating all contact items.

protocol ContactItemContentObserver

A protocol that defines a system observer that receives a resumable enumeration of all items.

