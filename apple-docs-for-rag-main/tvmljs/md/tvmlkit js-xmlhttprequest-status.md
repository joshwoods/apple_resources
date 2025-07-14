

- TVMLKit JS
- XMLHttpRequest
-  status 

Instance Property

# status

The HTTP status code.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 10.0+Safari Mobile 10.0+

**tvOS**

``` source
readonly attribute int status;
```

**Safari Desktop, Safari Mobile**

``` source
readonly attribute unsigned short status;
```

## Discussion

If the current state of the request is `unsent` or `opened`, then this attribute’s value is `0`.

## See Also

### Retrieving Request Information

metrics

A dictionary of keys used to request start and response start and end times.

readyState

The current state of the request.

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

statusText

The HTTP status text.

