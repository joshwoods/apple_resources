

- BrowserEngineKit
-  BEDownloadMonitor 

Class

# BEDownloadMonitor

An object that reports the status of web downloads to the system.

iOS 18.2+iPadOS 18.2+

``` source
@objc(BEDownloadMonitor)
class BEDownloadMonitor
```

## Mentioned in 

Downloading files in a web browser with an alternative browser engine

## Overview

When someone downloads a file in your web browser, create an instance of this class to report progress to the system, and optionally create a placeholder file in the person’s Downloads folder. For more information, see Downloading files in a web browser with an alternative browser engine.

## Topics

### Creating a download monitor

init(sourceURL: URL, destinationURL: URL, observedProgress: Progress, liveActivityAccessToken: Data)

Initializes a download monitor to report progress for the specified download.

static func createAccessToken() -> Data?

Generates an opaque token that the system uses to keep your networking extension active in the background.

### Creating a download placeholder

func useDownloadsFolder(placeholderType: UTType?, finalFileCreatedHandler: (BEDownloadMonitor.Location?) -> Void)

Asks the system to create a placeholder for the downloaded file in the person’s Downloads folder.

class Location

A class that associates a URL with the bookmark you use to access that URL.

### Reporting progress to the system

func beginMonitoring() async throws -> BEDownloadMonitor.Location?

Informs the system to start monitoring the download.

func resumeMonitoring(placeholderURL: URL) async throws

Informs the system that it needs to resume monitoring the download.

### Getting information about a download

let sourceURL: URL

let destinationURL: URL

### Identifying a download

let id: UUID

The stable identity of the entity associated with this instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- NSObjectProtocol
- Sendable

## See Also

### Downloads

Downloading files in a web browser with an alternative browser engine

Report download progress to the system to keep your networking extension active.

