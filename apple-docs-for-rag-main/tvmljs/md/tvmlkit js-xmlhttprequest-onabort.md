

- TVMLKit JS
- XMLHttpRequest
-  onabort 

Instance Property

# onabort

A callback function called when a request is cancelled by the user.

tvOS 9.0+

``` source
attribute function onabort;
```

## Discussion

This attribute must be set to a function; for example, `XMLHttpRequest.onabort = function () {}`.

## See Also

### Implementing Callback Functions

onerror

A callback function that is called if the request fails due to an error.

onload

A callback function that is called when the request is successfully completed.

onloadend

A callback function that is called when the request is completed for any reason.

onloadstart

A callback function that is called when the request begins.

onreadystatechange

A callback function that is called when the readyState attribute changes.

ontimeout

A callback function that is called when a request times out.

