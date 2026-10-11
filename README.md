# My Daily Tasks — Android project starter

A Kotlin + Jetpack Compose Android task list with auto-numbered rows, done checkbox, date/time picker, per-task alarm toggle, delete/reorder, and Room database persistence.

## Build
Open this folder in Android Studio (JDK 17, Android SDK 35) and let Gradle sync. Then Build > Build Bundle(s) / APK(s) > Build APK(s).

## Important reminder behavior / testing
This is a starter project and should be tested on a real Android phone before relying on it. Android exact-alarm and notification permissions vary by Android version and manufacturer. Android may delay inexact alarms under battery restrictions. The current reminder receiver is a baseline implementation; verify daily recurrence, reboot restoration, silent-mode behavior, and edit/cancel behavior on-device before everyday use. This source does not include a precompiled APK.
