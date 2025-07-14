

- BrowserEngineKit
- RestrictedSandboxAppliable
-  applyRestrictedSandbox(revision:) 

Instance Method

# applyRestrictedSandbox(revision:)

Puts a browser extension into a more restricted sandbox.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
func applyRestrictedSandbox(revision: RestrictedSandboxRevision)
```

**Required** Default implementations provided.

## Parameters 

`revision`  

The revision of the sandbox restriction rules to apply.

## Mentioned in 

Limiting resource access in web content extensions

## Default Implementations

### RestrictedSandboxAppliable Implementations

func applyRestrictedSandbox(revision: RestrictedSandboxRevision)

When called, the process will enter a restrictive sandbox mode.

func applyRestrictedSandbox(revision: RestrictedSandboxRevision)

When called, the process will enter a restrictive sandbox mode.

## See Also

### Applying sandbox restrictions

enum RestrictedSandboxRevision

Revisions to the restricted sandbox rules.

