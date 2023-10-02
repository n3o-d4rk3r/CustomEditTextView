# Upcomming CustomEditTextView Android Library

## Maintenance
In light of Material Design 3.0's release, continued support for this plugin is no longer a priority. It may receive minimal maintenance for minor bug fixes, but it doesn't align well with the new design guidelines. However, it is stable and functional as it stands.

## Instalation

Add jitpack.io in your top-level build.gradle:
```gradle
allprojects {
        repositories {
                ...
                maven { url 'https://jitpack.io' }
        }
}
```
Add the dependency:
```gradle
dependencies {
        implementation 'com.github.n3od4rk3r:CustomEditTextView:<Version Tag>'
}

```
Available versions:
| Release | Version Tag | Comment                     |
| ------- | ----------- | --------------------------- |
| legacy  | 1.0         | material [version <= 1.3.0] |
| stable  | 1.2         | material [version >= 1.4.0] |
| beta    | 1.1-beta6   | material [version >= 1.4.0] |

## Usage

Just add the view to your layout:
```xml

<com.yourpackage.CustomEditTextView
  android:layout_width="match_parent"
  android:layout_height="match_parent"
  .................................../>

```

The view is an extension to the material.io BottomNavigationView, and implements all it's functions.
The following custom properties are available:
```kotlin
navigationView.circleColor = Color.RED
navigationView.darkIcon = true
navigationView.backgroundShape = BottomNavigationView.Shape.RoundedRectangle
```
Or through XML:
```XML
app:circleColor="@color/red"
app:darkIcon="true"
app:backgroundShape="circle|roundedRectangle"
app:customBackgroundShape="@drawable/bg_custom"
```
