

- TVMLKit JS
- XMLHttpRequest
-  onloadstart 

Instance Property

# onloadstart

A callback function that is called when the request begins.

tvOS 9.0+

``` source
attribute function onloadstart;
```

## Discussion

This attribute must be set to a function; for example, `XMLHttpRequest.onloadstart = function () {}`.

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

onreadystatechange

A callback function that is called when the readyState attribute changes.

ontimeout

A callback function that is called when a request times out.

