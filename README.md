# Unity `runInBackground: 1` freeze

## Steps to produce builds

1. Using the Unity Hub (3.7.0), install Unity Editor 2022.3.24f1
2. Create a new project using the 2D (Built-in) template
3. Make a macOS build using the default build settings, call it `runInBackground-0`
4. Edit `ProjectSettings.asset` and change `runInBackground` to `1`
5. Make a second macOS build using the same build settings as before, call it `runInBackground-1`

## Testing steps

1. Open the build in fullscreen and repeatedly use command+tab to focus and blur the application
2. For a build containing the bug, the application will freeze on around the fourth attempt