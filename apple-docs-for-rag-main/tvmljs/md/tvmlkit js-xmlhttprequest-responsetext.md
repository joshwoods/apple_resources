

- TVMLKit JS
- XMLHttpRequest
-  responseText 

Instance Property

# responseText

The response to the request.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 9.0+Safari Mobile 9.0+

**tvOS**

``` source
readonly attribute String responseText;
```

**Safari Desktop, Safari Mobile**

``` source
readonly attribute DOMString? responseText;
```

## Discussion

If the request was unsuccessful or has not been sent, the value of this attribute is `null`. Otherwise, this attribute contains a string containing the response.

## See Also

### Retrieving Request Information

metrics

A dictionary of keys used to request start and response start and end times.

readyState

The current state of the request.

response

The response entity body.

responseCacheIsValid

responseType

The type of response.

responseURL

responseXML

The document response entity body.

status

The HTTP status code.

statusText

The HTTP status text.

