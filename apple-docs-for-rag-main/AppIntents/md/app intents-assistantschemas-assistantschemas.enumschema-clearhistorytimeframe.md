

- App Intents
- AssistantSchemas
- AssistantSchemas.EnumSchema
-  clearHistoryTimeFrame 

Instance Property

# clearHistoryTimeFrame

The time frame for clearing the browser history

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var clearHistoryTimeFrame: some AssistantSchemas.Enum { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app enum implementation.

For more information about the `.browser` app intent domain, see Making browser actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app enum that conforms to the `.browser.clearHistoryTimeFrame` schema:

```
@AssistantEnum(schema: .browser.clearHistoryTimeFrame)
enum ClearHistoryTimeFrame: AppEnum {

    case today
    case lastFourHours
    case todayAndYesterday
    case allTime

    static var caseDisplayRepresentations: [ClearHistoryTimeFrame: DisplayRepresentation] = [
        .today: "Today",
        .lastFourHours: "Last 4 hours",
        .todayAndYesterday: "Today and Yesterday",
        .allTime: "Beginning of time",
    ]

    static var typeDisplayName: LocalizedStringResource = "Clear History Timeframe"
}
```

