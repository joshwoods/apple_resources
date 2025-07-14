

- TVMLKit JS
- XMLHttpRequest
-  onload 

Instance Property

# onload

A callback function that is called when the request is successfully completed.

tvOS 9.0+

``` source
attribute function onload;
```

## Discussion

This attribute must be set to a function; for example, `XMLHttpRequest.onload = function () {}`.

## See Also

### Implementing Callback Functions

onabort

A callback function called when a request is cancelled by the user.

onerror

A callback function that is called if the request fails due to an error.

onloadend

A callback function that is called when the request is completed for any reason.

onloadstart

A callback function that is called when the request begins.

onreadystatechange

A callback function that is called when the readyState attribute changes.

ontimeout

A callback function that is called when a request times out.

