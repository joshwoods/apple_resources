

- Foundation
- URL
-  resourceBytes 

Instance Property

# resourceBytes

The URL’s resource data, as an asynchronous sequence of bytes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var resourceBytes: URL.AsyncBytes { get }
```

## Discussion

Use this property with Swift’s `for`-`await`-`in` syntax, to read the contents of a URL byte-by-byte, like this:

```
guard let url = URL(string: "https://www.example.com") else {
    return
}
do {
    // Read each byte of the data as it becomes available.
    for try await byte in url.resourceBytes
    {
        // Do something with byte.
    }
} catch {
    print ("Error: \(error)")
}
```

To wait for the entire resource to load, use the URLSession method data(from:delegate:) with the `await` keyword. URLSession also offers methods to upload data to a URL endpoint and download a URL’s contents to a file.

## See Also

### Loading URL contents asynchronously

var lines: AsyncLineSequence&lt;URL.AsyncBytes>

The URL’s resource data, as an asynchronous sequence of lines of text.

struct AsyncBytes

An asynchronous sequence of bytes loaded from the URL.

