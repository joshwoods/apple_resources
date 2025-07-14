

- TVMLKit JS
-  XMLHttpRequest 

Class

# XMLHttpRequest

An object used to retrieve data from a URL.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 10.0+Safari Mobile 3.0+

``` source
interface XMLHttpRequest
```

## Topics

### Initializing and Sending a Request

abort

Cancels any network activity.

open

Sets the method, URL, and synchronous flag for a request.

send

Sends the request.

timeout

The amount of time, in milliseconds, before causing a request to time out.

XMLHttpRequest

Creates a new XMLHttpRequest.

### Manipulating the Header List

getAllResponseHeaders

Returns all of the response headers.

getResponseHeader

Retrieves the field value from the response that is contained in the specified header.

setRequestHeader

Appends a header to the list of request headers.

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

status

The HTTP status code.

statusText

The HTTP status text.

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

onreadystatechange

A callback function that is called when the readyState attribute changes.

ontimeout

A callback function that is called when a request times out.

### Responding to Events

abort

An event signifying the request has aborted.

error

An event signifying an error occurred during the request.

load

An event signifying the request was successfully loaded.

loadend

An event signifying the request has been completed.

loadstart

An event signifying the request has begun.

readystatechange

An event signifying that a state change has occurred.

### WebKit JS Only

upload

withCredentials

overrideMimeType

retrieveResponse

UNSENT

OPENED

HEADERS_RECEIVED

LOADING

DONE

## Relationships

### Inherits From

- EventListenerObject
- XMLHttpRequestEventTarget

## See Also

### Data Storage and Retrieval

Binding JSON data to TVML documents

Create full-fledged TVML documents by using data binding and queries on simplified TVML files.

DataItem

An object used to create observable objects from JSON objects for data binding.

Storage

An object used to store key-value-pair information.

DataSource

An interface that allows the system to detect and respond to changes in your data.

LoadIndexesRequest

A request created when the loadindexes event is triggered.

