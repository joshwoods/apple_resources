

- TVMLKit JS
- XMLHttpRequest
-  readyState 

Instance Property

# readyState

The current state of the request.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 4.0+Safari Mobile 3.0+

**tvOS**

``` source
readonly attribute int readyState;
```

**Safari Desktop, Safari Mobile**

``` source
readonly attribute unsigned short readyState;
```

## Discussion

This attribute can have the following values:

- `0 - UNSENT`

- `1 - OPENED`

- `2 - HEADERS_RECEIVED`

- `3 - LOADING`

- `4 - DONE`

## See Also

### Retrieving Request Information

metrics

A dictionary of keys used to request start and response start and end times.

response

The response entity body.

responseCacheIsValid

responseText

The response to the request.

responseType

The type of response.

responseURL

responseXML

The document response entity body.

status

The HTTP status code.

statusText

The HTTP status text.

