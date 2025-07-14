

- Notary API
- NewSubmissionRequest
-  NewSubmissionRequest.Notifications 

Object

# NewSubmissionRequest.Notifications

A notification that the notary service sends you when notarization finishes.

Notary API 2.0.0+

``` source
object NewSubmissionRequest.Notifications
```

## Properties

`channel`

`string`

The channel that the service uses to notify you when notarization completes. The only supported value for this key is `webhook`.

`target`

`string`

The URL that the notary service accesses when notarization completes.

## Attributes 

Possible types:

## Mentioned in 

Submitting software for notarization over the web

## Discussion

If you want a notification when notarization completes, include a data structure of this type in the `notifications` array that’s part of the body when you post to the Submit Software endpoint. Set the value for the `channel` key to `webhook`, and provide a URL as the value for the `target` key. The service indicates when notarization finishes by posting a body to the URL like this:

```
```

The value for the `payload` key indicates when the operation starts and completes, as well as the submission ID and your Team ID. The submission ID matches the value that you receive in response to the Submit Software call. You can use the `signature` and `cert_chain` fields to verify the authenticity of the message against the Apple Inc. Root certificate that you can download from the Apple PKI site. If you need the certificate repeatedly, store a copy of the certificate on your server rather than downloading it every time you need it.

