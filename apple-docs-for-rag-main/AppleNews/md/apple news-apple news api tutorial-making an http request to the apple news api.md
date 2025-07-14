

- Apple News
- Apple News API Tutorial
-  Making an HTTP Request to the Apple News API 

Article

# Making an HTTP Request to the Apple News API

Create the URL, set the method, and send the request.

## Overview

You make an HTTP request to send or receive data from a server. On this page, you’ll make the HTTP request to the Apple News API to get details about the channel, including the name, corresponding website, and default section. See Read Channel Information.

**On this page, you’ll learn how to:**

- Create the URL `https://news-api.apple.com/channels/{channel-id}`.

- Set the method to `GET`.

- Send the request.

### Copy This Code

Open any text editor to copy this code. Save the file as `make_an_http_request.py`.

```
```

### Run the Script

Start the command prompt and change to the directory containing `make_an_http_request.py` file. Run this script to make an HTTP request to the Apple News API. This script takes Channel ID as an argument.

```
```

### Result

The script returns this error:

`{"errors":[{"code":"UNAUTHORIZED"}]}`

The error indicates that the HTTP request didn’t include the authorization header.

## See Also

### Apple News API Python Tutorial

Signing the HTTP Request

Sign the canonical request and send the custom authorization header to the Apple News API.

Publishing an Article

Build a URL and article body for the publish-article request.

