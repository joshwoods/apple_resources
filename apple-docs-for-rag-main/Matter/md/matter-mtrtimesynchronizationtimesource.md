

- Matter
-  MTRTimeSynchronizationTimeSource 

Enumeration

# MTRTimeSynchronizationTimeSource

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
enum MTRTimeSynchronizationTimeSource
```

## Topics

### Enumeration Cases

case admin

case cloudSource

case nodeTimeCluster

case none

case unknown

case GNSS

case PTP

case matterNTP

case matterNTPNTS

case matterSNTP

case matterSNTPNTS

case mixedNTP

case mixedNTPNTS

case nonMatterNTP

case nonMatterNTPNTS

case nonMatterSNTP

case nonMatterSNTPNTS

### Type Properties

static var fabricNtp: MTRTimeSynchronizationTimeSource

static var fabricNtpNts: MTRTimeSynchronizationTimeSource

static var fabricSntp: MTRTimeSynchronizationTimeSource

static var fabricSntpNts: MTRTimeSynchronizationTimeSource

static var gnss: MTRTimeSynchronizationTimeSource

static var mixedNtp: MTRTimeSynchronizationTimeSource

static var mixedNtpNts: MTRTimeSynchronizationTimeSource

static var nonFabricNtp: MTRTimeSynchronizationTimeSource

static var nonFabricNtpNts: MTRTimeSynchronizationTimeSource

static var nonFabricSntp: MTRTimeSynchronizationTimeSource

static var nonFabricSntpNts: MTRTimeSynchronizationTimeSource

static var ptp: MTRTimeSynchronizationTimeSource

### Initializers

init?(rawValue: UInt8)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

