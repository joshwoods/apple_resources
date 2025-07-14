

- TVMLKit JS
- XMLHttpRequest
-  timeout 

Instance Property

# timeout

The amount of time, in milliseconds, before causing a request to time out.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 9.0+Safari Mobile 9.0+

**tvOS**

``` source
attribute int timeout;
```

**Safari Desktop, Safari Mobile**

``` source
attribute unsigned long timeout;
```

## Discussion

This attribute only takes effect if the request is asynchronous. When set to `0`, the request will not automatically time out.

## See Also

### Initializing and Sending a Request

abort

Cancels any network activity.

open

Sets the method, URL, and synchronous flag for a request.

send

Sends the request.

XMLHttpRequest

Creates a new XMLHttpRequest.

