

- App Intents
-  AppEntityAnnotatable 

Protocol

# AppEntityAnnotatable

A protocol that framework types adopt to enable you to provide content to system experiences.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
protocol AppEntityAnnotatable
```

## Overview

Do not declare new conformances to `AppEntityAnnotatable`. Framework types like NSUserActivity conform to the protocol to enable you to make your app’s content available to system experiences, including Siri and Apple Intelligence.

## Topics

### Instance Properties

var appEntityIdentifier: EntityIdentifier?

The identifier of an app entity you set on framework types to make app content available to system experiences.

**Required**

