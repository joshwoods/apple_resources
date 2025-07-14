

- Foundation
- NSURLDownload
-  cancel() 

Instance Method

# cancel()

Cancels the receiver’s download and deletes the downloaded file.

macOS 10.2+

``` source
func cancel()
```

## Discussion

This method deletes the partially downloaded file unless you have previously called deletesFileUponFailure, passing false.

