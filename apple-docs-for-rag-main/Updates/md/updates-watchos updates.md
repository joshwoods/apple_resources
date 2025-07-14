

- Updates
-  watchOS updates 

Article

# watchOS updates

Learn about important changes to watchOS.

## Overview

Browse notable changes in watchOS apps.

## September 2024

### Watch sizes

- Apple Watch Series 10 are larger and have a different aspect ratio than previous watches. The watch is 1mm larger than the Series 9 (42mm and 46mm), but the screen gains more width than height. Use scenePadding(_:) to align text with the text margins, and ignoresSafeArea(_:edges:) to extend content beyond the watch’s safe area.

### Shallow dives

- Apple Watch Series 10 supports the Shallow Depth and Pressure capability. Use CMWaterSubmersionManager to start a shallow dive session, and underwaterDepth and waterTemperature to read depth and temperature samples from HealthKit.

## June 2024

### Water temperature

- Access water temperature data from swimming workouts. Apple Watch Ultra records waterTemperature samples during swimming workouts.

### Double tap

- Specify which control responds to the double tap gesture using the handGestureShortcut(_:isEnabled:) view modifier, passing primaryAction as the parameter. Double tap can interact with any buttonlike controls, such as buttons or toggles.

### Creating workouts

- Create custom pool swimming workouts with the HKWorkoutActivityType.swimming activity.

- Set a distance-with-time goal for custom swimming workouts with the WorkoutGoal.poolSwimDistanceWithTime(_:_:) goal.

- Provide a custom name to a workout step using the WorkoutStep structure’s displayName.

- Preview workouts on Apple Watch using the workoutPreview(_:isPresented:) view modifier.

- Set average power goals for cycling and running with PowerThresholdAlert and PowerRangeAlert.

- Set pace goals for indoor running with the SpeedThresholdAlert and SpeedRangeAlert targets.

## September 2023

- When someone performs a Double Tap gesture while viewing a notification on Apple Watch Series 9 or Apple Watch Ultra 2, the system invokes the first nondestructive action. A nondestructive action doesn’t include the destructive option, and won’t delete user data or change the app irrevocably.

## June 2023

- Use the new watchOS user interface design to simplify navigation, better use the Digital Crown, and enrich the app experience. For more information, see Designing for watchOS and Creating an intuitive and effective UI in watchOS 10.

- Update your WidgetKit-based complications to take advantage of the Smart Stack on Apple Watch. People can scroll down to see relevant widgets directly on the watch face using the Digital Crown. For more information, see Increasing the visibility of widgets in Smart Stacks.

- Use curved text along the bevel or around the corners in WidgetKit-based complications.

- Add state preservation and restoration to watchOS apps. For more information, see Preserving your app’s UI across launches.

- Use WorkoutKit to create goal, pacer, multisport, and fully custom interval workouts. Display a preview of the workout that shows the workout details, and sync workouts with a paired Apple Watch. For more information, see WorkoutKit.

- Access batches of high-frequency accelerometer and device motion data during workouts. Use this data to analyze motion — such as a golf or baseball swing — after the action occurs. For more information, see Core Motion.

- Use Core Motion’s water submersion manager to monitor shallow dives on Apple Watch Ultra. For more information, see Core Motion.

- Support Bluetooth cycling sensors. People can pair power, cadence, and speed sensors to Apple Watch to enhance their cycling workouts. You can access this data using HealthKit for live and historical workouts.

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

App Intents updates

Learn about important changes in App Intents.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AuthenticationServices updates

Learn about important changes to AuthenticationServices.

AVFAudio updates

Learn about important changes to AVFAudio.

AVFoundation updates

Learn about important changes to AVFoundation.

Bundle Resources updates

Learn about important changes to Bundle Resources.

ContactsUI updates

Learn about important changes to ContactsUI.

