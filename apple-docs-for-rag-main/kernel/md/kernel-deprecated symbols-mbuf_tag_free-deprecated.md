

- Kernel
- Deprecated Symbols
-  mbuf_tag_free Deprecated

Function

# mbuf_tag_free

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_tag_free(mbuf_t mbuf, mbuf_tag_id_t module_id, mbuf_tag_type_t type);
```

## Parameters 

`mbuf`  

The mbuf the tag was allocated on.

`module_id`  

The ID of the tag to free.

`type`  

The type of the tag to free.

## Discussion

Frees a previously allocated mbuf tag.

