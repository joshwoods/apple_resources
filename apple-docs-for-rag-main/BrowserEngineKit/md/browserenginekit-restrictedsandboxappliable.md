

- BrowserEngineKit
-  RestrictedSandboxAppliable 

Protocol

# RestrictedSandboxAppliable

A protocol that browser extensions implement to opt into a more restricted sandbox.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
protocol RestrictedSandboxAppliable
```

## Mentioned in 

Limiting resource access in web content extensions

## Overview

Call applyRestrictedSandbox(revision:) to enter the restricted sandbox, indicating which revision of the sandbox restrictions to apply. In revision 1, corresponding to RestrictedSandboxRevision.revision1, additional restrictions affect the web content extension only. For more information, see Limiting resource access in web content extensions.

## Topics

### Applying sandbox restrictions

func applyRestrictedSandbox(revision: RestrictedSandboxRevision)

Puts a browser extension into a more restricted sandbox.

**Required** Default implementations provided.

enum RestrictedSandboxRevision

Revisions to the restricted sandbox rules.

## Relationships

### Inherited By

- NetworkingExtension
- RenderingExtension
- WebContentExtension

## See Also

### Access control

Limiting resource access in web content extensions

Reduce the impact of vulnerabilities in web content extensions by limiting privileges.

Accessing files in browser extensions

Grant extensions access to files from within your browser app.

Attributing memory to a content extension

Adhere to operating-system limits on GPU memory use.

enum RestrictedSandboxRevision

Revisions to the restricted sandbox rules.

