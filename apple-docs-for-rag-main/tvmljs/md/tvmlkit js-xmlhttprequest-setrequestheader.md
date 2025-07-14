

- TVMLKit JS
- XMLHttpRequest
-  setRequestHeader 

Instance Method

# setRequestHeader

Appends a header to the list of request headers.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 4.0+Safari Mobile 3.0+

**tvOS**

``` source
void setRequestHeader(
    in String header, 
    in String value
);
```

**Safari Desktop, Safari Mobile**

``` source
void setRequestHeader(
    DOMString header, 
    DOMString value
);
```

## Parameters 

`header`  

The header name.

`value`  

The header value.

## Discussion

If the header already exists in the list of request headers, the specified value is combined with the value currently in the list to create a single request header.

## See Also

### Manipulating the Header List

getAllResponseHeaders

Returns all of the response headers.

getResponseHeader

Retrieves the field value from the response that is contained in the specified header.

