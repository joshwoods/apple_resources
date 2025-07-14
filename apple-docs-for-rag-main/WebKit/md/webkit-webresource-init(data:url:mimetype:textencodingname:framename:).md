

- WebKit
- WebResource
-  init(data:url:mimeType:textEncodingName:frameName:) 

Initializer

# init(data:url:mimeType:textEncodingName:frameName:)

Initializes and returns a web resource instance.

macOS

``` source
init!(
    data: Data!,
    url URL: URL!,
    mimeType MIMEType: String!,
    textEncodingName: String!,
    frameName: String!
)
```

## Parameters 

`data`  

The download data.

`URL`  

The download URL.

`MIMEType`  

The MIME type of the data.

`textEncodingName`  

The IANA encoding name (for example, “utf-8” or “utf-16”). This parameter may be `nil`.

`frameName`  

The name of the frame. Use this parameter if the resource represents the contents of an entire HTML frame; otherwise pass `nil`.

## Return Value

An initialized web resource.

