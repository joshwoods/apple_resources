

- Kernel
- Kernel Functions
-  kev_msg_post 

Function

# kev_msg_post

macOS 10.9+

``` source
errno_t kev_msg_post(struct kev_msg *event_msg);
```

## Parameters 

`event_msg`  

A structure defining the kernel event message to post.

## Return Value

Will return zero upon success. May return a number of errors depending on the type of failure. EINVAL indicates that there was something wrong with the kerne event. The vendor code of the kernel event must be assigned using kev_vendor_code_find. If the message is too large, EMSGSIZE will be returned.

## Discussion

Post a kernel event message.

