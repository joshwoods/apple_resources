

- App Intents
- IntentPredictionsBuilder
-  buildBlock(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Type Method

# buildBlock(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildBlock(
    _ a0: A0,
    _ a1: A1,
    _ a2: A2,
    _ a3: A3,
    _ a4: A4,
    _ a5: A5,
    _ a6: A6,
    _ a7: A7,
    _ a8: A8
) -> TupleIntentPrediction where Intent == A0.Intent, A0 : IntentPredictionConfiguration, A1 : IntentPredictionConfiguration, A2 : IntentPredictionConfiguration, A3 : IntentPredictionConfiguration, A4 : IntentPredictionConfiguration, A5 : IntentPredictionConfiguration, A6 : IntentPredictionConfiguration, A7 : IntentPredictionConfiguration, A8 : IntentPredictionConfiguration, A0.Intent == A1.Intent, A1.Intent == A2.Intent, A2.Intent == A3.Intent, A3.Intent == A4.Intent, A4.Intent == A5.Intent, A5.Intent == A6.Intent, A6.Intent == A7.Intent, A7.Intent == A8.Intent
```

Available when `Intent` conforms to `AppIntent`.

