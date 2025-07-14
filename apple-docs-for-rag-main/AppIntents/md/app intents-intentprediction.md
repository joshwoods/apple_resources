

- App Intents
-  IntentPrediction 

Structure

# IntentPrediction

A prediction for a specific app intent that the system might display to someone when it’s relevant.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentPrediction where Intent : AppIntent
```

## Overview

Includes the predicted parameters, and ways to get a user-visible description for a predicted or suggested action given those parameters.

## Topics

### Creating a prediction

init(displayRepresentation: () -> DisplayRepresentation)

### Initializers

init&lt;V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11, P0, P1, P2, P3, P4, P5, P6, P7, P8, P9, P10, P11, K0, K1, K2, K3, K4, K5, K6, K7, K8, K9, K10, K11>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, P0, P1, P2, P3, P4, P5, P6, P7, P8, P9, P10, K0, K1, K2, K3, K4, K5, K6, K7, K8, K9, K10>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, V5, P0, P1, P2, P3, P4, P5, K0, K1, K2, K3, K4, K5>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11, V12, V13, V14, P0, P1, P2, P3, P4, P5, P6, P7, P8, P9, P10, P11, P12, P13, P14, K0, K1, K2, K3, K4, K5, K6, K7, K8, K9, K10, K11, K12, K13, K14>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11, V12, V13, V14) -> DisplayRepresentation)

init&lt;V0, V1, P0, P1, K0, K1>(parameters: T, displayRepresentation: (V0, V1) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, P0, P1, P2, P3, P4, P5, P6, P7, P8, P9, K0, K1, K2, K3, K4, K5, K6, K7, K8, K9>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5, V6, V7, V8, V9) -> DisplayRepresentation)

init&lt;V0, P0>(parameters: T, displayRepresentation: (V0) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11, V12, P0, P1, P2, P3, P4, P5, P6, P7, P8, P9, P10, P11, P12, K0, K1, K2, K3, K4, K5, K6, K7, K8, K9, K10, K11, K12>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11, V12) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, P0, P1, P2, P3, P4, K0, K1, K2, K3, K4>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, V5, V6, V7, P0, P1, P2, P3, P4, P5, P6, P7, K0, K1, K2, K3, K4, K5, K6, K7>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5, V6, V7) -> DisplayRepresentation)

init&lt;V0, V1, V2, P0, P1, P2, K0, K1, K2>(parameters: T, displayRepresentation: (V0, V1, V2) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, V5, V6, P0, P1, P2, P3, P4, P5, P6, K0, K1, K2, K3, K4, K5, K6>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5, V6) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, V5, V6, V7, V8, P0, P1, P2, P3, P4, P5, P6, P7, P8, K0, K1, K2, K3, K4, K5, K6, K7, K8>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5, V6, V7, V8) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, P0, P1, P2, P3, K0, K1, K2, K3>(parameters: T, displayRepresentation: (V0, V1, V2, V3) -> DisplayRepresentation)

init&lt;V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11, V12, V13, P0, P1, P2, P3, P4, P5, P6, P7, P8, P9, P10, P11, P12, P13, K0, K1, K2, K3, K4, K5, K6, K7, K8, K9, K10, K11, K12, K13>(parameters: T, displayRepresentation: (V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11, V12, V13) -> DisplayRepresentation)

## Relationships

### Conforms To

- IntentPredictionConfiguration

## See Also

### Intent predictions

protocol PredictableIntent

An interface that allows the system to suggest the app intent to someone in the future using predictions you provide.

