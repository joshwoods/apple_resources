

- Social
- SLRequest
-  addMultipartData(\_:withName:type:filename:) 

Instance Method

# addMultipartData(\_:withName:type:filename:)

Specifies a named multipart POST body for this request.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+

``` source
func addMultipartData(
    _ data: Data!,
    withName name: String!,
    type: String!,
    filename: String!
)
```

## Parameters 

`data`  

The data for the multipart POST body, such as an image or text.

`name`  

The name of the multipart POST body. This is the name that a specific social service expects.

`type`  

The type of the multipart POST body. This is the MIME content type of the multipart data.

`filename`  

The filename of the attachment that you want to POST. Many social services require a filename in order to accept certain POST requests, such as uploading an image or video. If your multipart data does not require a filename, pass in `nil`.

## Discussion

Possible parameter values are dependent on the target service. This information, as well as guidance on when to use a multipart POST body, is documented by the service provider. For links to documentation for the supported services, see Table 1 in SLRequest.

## See Also

### Adding Data to the Request

func addMultipartData(Data!, withName: String!, type: String!)

Specifies a named multipart POST body for this request.

Deprecated

