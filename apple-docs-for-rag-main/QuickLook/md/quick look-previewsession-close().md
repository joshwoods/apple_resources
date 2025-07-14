

- Quick Look
- PreviewSession
-  close() 

Instance Method

# close()

Closes the preview session.

visionOS 2.0+

``` source
func close() async throws
```

## Discussion

If the existing session is still open, this method closes it. The session’s events stream receives a `.didClose` event upon success.

Throws

An `Error` if it is not possible to close the PreviewSession.

