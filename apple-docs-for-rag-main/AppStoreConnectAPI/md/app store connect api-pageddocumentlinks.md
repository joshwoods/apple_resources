

- App Store Connect API
-  PagedDocumentLinks 

Object

# PagedDocumentLinks

Links related to the response document, including paging links.

App Store Connect API 1.0+

``` source
object PagedDocumentLinks
```

## Properties

`first`

`uri-reference`

The link to the first page of documents.

`next`

`uri-reference`

The link to the next page of documents.

`self`

`uri-reference`

 (Required) 

The link that produced the current document.

## Discussion

All the response data constitutes multiple *documents.*

## See Also

### Objects

object PagingInformation

Paging information for data responses.

object ResourceLinks

Self-links to requested resources.

object DocumentLinks

Self-links to documents that can contain information for one or more resources.

object RelationshipLinks

Links related to the response document, including self links.

