

- Wallet Orders
-  Receive log messages 

Web Service Endpoint

# Receive log messages

Records log messages on your server.

iOS 16.0+iPadOS 16.0+macOS 13.0+

## URL

``` source
POST https://your-web-service.com/v1/log
```

## HTTP Body

LogEntries

An array of log messages.

Content-Type: application/json

## Response Codes

` 200 ``OK`

`OK`

The request was successful.

## See Also

### Message logs

object LogEntries

An array of log messages.

