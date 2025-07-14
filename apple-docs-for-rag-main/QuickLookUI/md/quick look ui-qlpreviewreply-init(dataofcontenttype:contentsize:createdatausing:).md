

- Quick Look UI
- QLPreviewReply
-  init(dataOfContentType:contentSize:createDataUsing:) 

Initializer

# init(dataOfContentType:contentSize:createDataUsing:)

macOS 12.0+

``` source
convenience init(
    dataOfContentType contentType: UTType,
    contentSize: CGSize,
    createDataUsing closure: @escaping (QLPreviewReply) throws -> Data
)
```

