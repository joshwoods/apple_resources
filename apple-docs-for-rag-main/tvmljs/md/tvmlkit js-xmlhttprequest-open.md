

- TVMLKit JS
- XMLHttpRequest
-  open 

Instance Method

# open

Sets the method, URL, and synchronous flag for a request.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 4.0+Safari Mobile 3.0+

**tvOS**

``` source
void open(
    in String method, 
    in String urlStr, 
    in optional int asyncNum, 
    in optional Object user, 
    in optional Object password
);
```

**Safari Desktop, Safari Mobile**

``` source
void open(
    DOMString method, 
    DOMString url
);
```

## Parameters 

`method`  

The HTTP method for the request. `connect`, `trace`, and `track` are invalid values.

`urlStr`  

The URL for the request.

`asyncNum`  

An integer value indicating if the request is asynchronous. `0` is a synchronous request. Any positive integer is an asynchronous request. The default value is `1`.

`user`  

Not supported by Apple TV. This value must be set to `null`.

`password`  

Not supported by Apple TV. This value must be set to `null`.

## Discussion

This method initializes a request.

## See Also

### Initializing and Sending a Request

abort

Cancels any network activity.

send

Sends the request.

timeout

The amount of time, in milliseconds, before causing a request to time out.

XMLHttpRequest

Creates a new XMLHttpRequest.

