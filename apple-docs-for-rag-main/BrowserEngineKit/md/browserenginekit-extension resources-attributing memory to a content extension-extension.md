

- BrowserEngineKit
- Extension resources
-  Attributing memory to a content extension 

Article

# Attributing memory to a content extension

Adhere to operating-system limits on GPU memory use.

## Overview

A web browser’s GPU extension is limited to a small total memory allocation. To allocate large amounts of memory in a GPU extension on behalf of a content extension, attribute the memory to that content extension.

The GPU and the content extension both need specific memory transfer entitlements to participate in memory attribution. In the content extension, you create a token that identifies the extension to the kernel. Pass the token to the GPU using your interprocess communication (IPC) channel. Then, in the GPU extension, use the token to assign ownership of the memory region to the content process.

## Use the correct entitlements

To participate in memory attribution, your content extension needs both the web-browser content extension entitlement `com.apple.developer.web-browser-engine.webcontent` and the `com.apple.developer.memory.transfer_accept` entitlement.

Your GPU extension needs both the `com.apple.developer.web-browser-engine.rendering` and `com.apple.developer.memory.transfer_send` entitlements.

Set the value for each of these entitlements to a string that matches the bundle ID of your browser app.

For more information about the entitlements web browser extensions use, see Designing your browser architecture.

## Create a task identity token

Your content extension creates a task identity token that you pass to the GPU extension using your IPC protocol, for example, with XPC. The task identity token is an unforgeable value that the operating system uses to identify the process to which it attributes memory in the GPU extension.

To create a task identity token:

```
```

## Attribute memory to the content extension

Receive the task identity token in the GPU extension and use it to attribute memory to the content extension.

To attribute an IOSurfaceRef to a content extension, call `IOSurfaceSetOwnershipIdentity`:

```
```

To attribute a `MTLResource` to a content extension, send it a `setOwnerWithIdentity:` message:

```
```

## Free the memory when the content extension finishes

When the content extension exits, whether normally or due to an error, free the memory that’s attributed to it in your GPU extension.

If you use `libxpc` to implement your IPC protocol, use the connection’s invalidation handler to detect when the content extension exits.

## See Also

### Access control

Limiting resource access in web content extensions

Reduce the impact of vulnerabilities in web content extensions by limiting privileges.

Accessing files in browser extensions

Grant extensions access to files from within your browser app.

protocol RestrictedSandboxAppliable

A protocol that browser extensions implement to opt into a more restricted sandbox.

enum RestrictedSandboxRevision

Revisions to the restricted sandbox rules.

