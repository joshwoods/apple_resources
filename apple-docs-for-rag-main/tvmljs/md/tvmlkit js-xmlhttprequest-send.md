

- TVMLKit JS
- XMLHttpRequest
-  send 

Instance Method

# send

Sends the request.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 4.0+Safari Mobile 3.0+

**tvOS**

``` source
void send(
    in Object dataToSend
);
```

**Safari Desktop, Safari Mobile**

``` source
void send();
```

## Parameters 

`dataToSend`  

The data sent.

## Discussion

For asynchronous requests, this function immediately returns control back to the app. Synchronous requests don’t return control back to the app until the response has arrived.

## See Also

### Initializing and Sending a Request

abort

Cancels any network activity.

open

Sets the method, URL, and synchronous flag for a request.

timeout

The amount of time, in milliseconds, before causing a request to time out.

XMLHttpRequest

Creates a new XMLHttpRequest.

