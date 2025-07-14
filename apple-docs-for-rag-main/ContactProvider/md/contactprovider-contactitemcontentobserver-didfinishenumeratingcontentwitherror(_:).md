

- ContactProvider
- ContactItemContentObserver
-  didFinishEnumeratingContentWithError(\_:) 

Instance Method

# didFinishEnumeratingContentWithError(\_:)

Finishes the content enumeration with an error, indicating failure, to the observer.

iOS 18.0+iPadOS 18.0+

``` source
func didFinishEnumeratingContentWithError(_: any Error)
```

**Required**

## Discussion

Use ContactProviderError.pageExpired to restart the content enumeration.

## See Also

### Ending enumeration

func didFinishEnumeratingContent(upTo: Data)

Finishes the content enumeration to the observer.

**Required**

func didFinishEnumeratingPage(upTo: ContactItemPage)

Marks a page of items as completed.

**Required**

struct ContactItemPage

A fixed offset into enumerating all contact items.

