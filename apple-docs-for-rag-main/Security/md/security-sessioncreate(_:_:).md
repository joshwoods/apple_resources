

- Security
-  SessionCreate(\_:\_:) 

Function

# SessionCreate(\_:\_:)

Creates a security session.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SessionCreate(
    _ flags: SessionCreationFlags,
    _ attributes: SessionAttributeBits
) -> OSStatus
```

## Parameters 

`flags`  

Flags controlling how the session is created. See SessionCreationFlags for valid values.

`attributes`  

The set of attribute bits to set for the new session. Not all bits can be set this way. See SessionAttributeBits for valid values.

## Return Value

A result code. See Sessions API Result Codes.

## Discussion

Upon completion, the new session contains the calling process (and none other). You can’t create a session for someone else, and can’t avoid being placed into the new session. This is (currently) the only call that changes a process’s session membership.

By default, a new bootstrap subset port is created for the calling process. The process acquires this new port as its bootstrap port, which all its children will inherit. If you happen to have created the subset port on your own, you can pass the sessionKeepCurrentBootstrap flag, and SessionCreate(_:_:) will use it. Note however that you cannot supersede a prior SessionCreate(_:_:) call that way; only a single SessionCreate(_:_:) call is allowed for each session (however made).

This call will discard any security information established for the calling process. In particular, any authorization handles acquired will become invalid, and so will any keychain related information. Call SessionCreate(_:_:) before making any other security-related calls that establish rights of any kind, to the extent this is practical. Also, do not perform security-related calls in any other threads while calling SessionCreate(_:_:).

