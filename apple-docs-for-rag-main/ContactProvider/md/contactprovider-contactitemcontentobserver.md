

- ContactProvider
-  ContactItemContentObserver 

Protocol

# ContactItemContentObserver

A protocol that defines a system observer that receives a resumable enumeration of all items.

iOS 18.0+iPadOS 18.0+

``` source
protocol ContactItemContentObserver
```

## Overview

Your implementation of enumerateContent(in:for:) receives an observer that conforms to this type. As you enumerate over your contact items, you provide them to the observer with the didEnumerate(_:) method.

## Topics

### Providing contact items

func didEnumerate([ContactItem])

Provides an array of contact items to the observer.

**Required**

enum ContactItem

An item in the contact database.

### Ending enumeration

func didFinishEnumeratingContent(upTo: Data)

Finishes the content enumeration to the observer.

**Required**

func didFinishEnumeratingPage(upTo: ContactItemPage)

Marks a page of items as completed.

**Required**

struct ContactItemPage

A fixed offset into enumerating all contact items.

func didFinishEnumeratingContentWithError(any Error)

Finishes the content enumeration with an error, indicating failure, to the observer.

**Required**

### Optimizing enumeration

var suggestedPageSize: Int

Retrieves the suggested number of items to include in a page.

**Required**

## See Also

### Receiving contacts

protocol ContactItemChangeObserver

A protocol that defines a system observer that receives a resumable enumeration of changed contact items.

