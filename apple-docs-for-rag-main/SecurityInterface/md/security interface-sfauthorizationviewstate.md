

- Security Interface
-  SFAuthorizationViewState 

Structure

# SFAuthorizationViewState

Defines the current state of the authorization view.

macOS 10.3+

``` source
struct SFAuthorizationViewState
```

## Overview

These constants are described in Constants in SFAuthorizationView.

## Topics

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

### Constants

var SFAuthorizationStartupState: SFAuthorizationViewState

Indicates that the state is starting up

var SFAuthorizationViewInProgressState: SFAuthorizationViewState

Indicates that the state is in progress

var SFAuthorizationViewLockedState: SFAuthorizationViewState

Indicates that the state is locked

var SFAuthorizationViewUnlockedState: SFAuthorizationViewState

Indicates that the state is unlocked

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Reference

struct SFButtonType

These constants define the button types used by authorization plug-ins.

struct SFViewType

These constants define the view type requested by the authorization plug-in.

SecurityInterface Constants

Constants in the SecurityInterface framework.

SecurityInterface Data Types

Data types found in the Security Interface framework.

SecurityInterface Enumerations

