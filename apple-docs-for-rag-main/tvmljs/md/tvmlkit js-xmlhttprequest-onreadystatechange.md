

- TVMLKit JS
- XMLHttpRequest
-  onreadystatechange 

Instance Property

# onreadystatechange

A callback function that is called when the readyState attribute changes.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 10.0+Safari Mobile 10.0+

**tvOS**

``` source
attribute function onreadystatechange;
```

**Safari Desktop, Safari Mobile**

``` source
attribute EventHandler onreadystatechange;
```

## Discussion

Do not use this attribute in conjunction with synchronous requests. This attribute must be set to a function; for example, `XMLHttpRequest.onreadystatechange = function () {}`.

## See Also

### Implementing Callback Functions

onabort

A callback function called when a request is cancelled by the user.

onerror

A callback function that is called if the request fails due to an error.

onload

A callback function that is called when the request is successfully completed.

onloadend

A callback function that is called when the request is completed for any reason.

onloadstart

A callback function that is called when the request begins.

ontimeout

A callback function that is called when a request times out.

