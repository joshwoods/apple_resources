

- ContactProvider
-  ContactItemPage 

Structure

# ContactItemPage

A fixed offset into enumerating all contact items.

iOS 18.0+iPadOS 18.0+

``` source
struct ContactItemPage
```

## Overview

You can break an enumeration of all contact items into multiple pages to reduce the memory constraints on the system. During the enumeration, the generationMarker must not change. Update the offset to reflect progress so you can resume the enumeration.

## Topics

### Creating a contact item page

init(generationMarker: Data, offset: Int)

Creates a contact item page with the given generation marker and offset.

### Supporting paging

var generationMarker: Data

A value specific to your data source identifying the database generation when enumeration of content started.

var offset: Int

An offset from the page’s generation marker.

static let initialPage: ContactItemPage

A static value the system uses to indicate the start of a new content enumeration.

### Encoding and decoding

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Comparing contact item pages

static func == (ContactItemPage, ContactItemPage) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable

## See Also

### Ending enumeration

func didFinishEnumeratingContent(upTo: Data)

Finishes the content enumeration to the observer.

**Required**

func didFinishEnumeratingPage(upTo: ContactItemPage)

Marks a page of items as completed.

**Required**

func didFinishEnumeratingContentWithError(any Error)

Finishes the content enumeration with an error, indicating failure, to the observer.

**Required**

