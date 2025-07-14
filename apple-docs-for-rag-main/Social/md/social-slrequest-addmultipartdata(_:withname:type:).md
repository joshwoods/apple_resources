

- Social
- SLRequest
-  addMultipartData(\_:withName:type:) 

Instance Method

# addMultipartData(\_:withName:type:)

Specifies a named multipart POST body for this request.

macOS 10.8+

``` source
func addMultipartData(
    _ data: Data!,
    withName name: String!,
    type: String!
)
```

## Parameters 

`data`  

The data for the multipart POST body, such as an image or text.

`name`  

The name of the multipart POST body. This is the name that a specific social service expects.

`type`  

The type of the multipart POST body. This is the MIME content type of the multipart data.

## Discussion

Possible parameter values are dependent on the target service. This information, as well as guidance on when to use a multipart POST body, is documented by the service provider. For links to documentation for the supported services, see Table 1 in SLRequest.

## See Also

### Adding Data to the Request

func addMultipartData(Data!, withName: String!, type: String!, filename: String!)

Specifies a named multipart POST body for this request.

