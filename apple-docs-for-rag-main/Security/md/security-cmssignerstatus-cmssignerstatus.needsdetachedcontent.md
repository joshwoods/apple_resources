

- Security
- CMSSignerStatus
-  CMSSignerStatus.needsDetachedContent 

Case

# CMSSignerStatus.needsDetachedContent

The message was signed but has detached content. You must call the CMSDecoderSetDetachedContent(_:_:) function before ascertaining the signature status.

Mac Catalyst 13.0+macOS 10.0+

``` source
case needsDetachedContent
```

