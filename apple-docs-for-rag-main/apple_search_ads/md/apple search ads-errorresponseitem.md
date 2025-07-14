

- Apple Search Ads
-  ErrorResponseItem 

Object

# ErrorResponseItem

The error response details in the response body.

Search Ads 2.0+

``` source
object ErrorResponseItem
```

## Properties

`field`

`string`

The details regarding an error.

`message`

`string`

A nonlocalized (U.S. English only) user-friendly string that describes the error.

`messageCode`

`string`

A system-assigned error code.

## Discussion

```
{
   "errors": [
     {
       "messageCode": "404",
       "message": "Not Found: The API can’t locate the resource.",
       "field": "null"
     },
   ...
   ]
}

```

## See Also

### Error Responses

object ApiErrorResponse

A parent object of the error response body.

object ErrorResponseBody

A parent object of the error response.

object IntegerResponse

A common integer type response.

object VoidResponse

A default generic null response.

