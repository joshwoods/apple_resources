

- TVMLKit JS
- XMLHttpRequest
-  getAllResponseHeaders 

Instance Method

# getAllResponseHeaders

Returns all of the response headers.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 10.0+Safari Mobile 10.0+

**tvOS**

``` source
String getAllResponseHeaders();
```

**Safari Desktop, Safari Mobile**

``` source
DOMString getAllResponseHeaders();
```

## Return Value

A string representation of the response headers.

## Discussion

Returns `null` if no responses have been received.

## See Also

### Manipulating the Header List

getResponseHeader

Retrieves the field value from the response that is contained in the specified header.

setRequestHeader

Appends a header to the list of request headers.

