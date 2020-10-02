# DDAnimatoo

[![platform](https://img.shields.io/badge/platform-Android-yellow.svg)](https://www.android.com)
[![API](https://img.shields.io/badge/API-16%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=16)
[ ![Download](https://api.bintray.com/packages/dd4you/DD4YouAppsConfig/in.dd4you.animatoo/images/download.svg) ](https://bintray.com/dd4you/DD4YouAppsConfig/in.dd4you.animatoo/_latestVersion)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg?style=flat-square)](https://www.apache.org/licenses/LICENSE-2.0.html)


Bored with same animation for activity, Fragment, ViewPager and Viewpager2 transition? DDAnimatoo is a lightweight and easy to use Android library that provides many activity, Fragment, ViewPager and Viewpager2 transition animations.
* min SDK 16 (Android Jellybean 4.1)
* written in Java

A lightweight, easy-to-use Android library that provides awesome activity, Fragment, ViewPager and Viewpager2 transition animations


## Screenshots
<img src="https://github.com/DD4You/DDAnimatoo/blob/master/screenshots/activity.gif" width="190" height="270" />
<img src="https://github.com/DD4You/DDAnimatoo/blob/master/screenshots/fragment.gif" width="190" height="270" />
<img src="https://github.com/DD4You/DDAnimatoo/blob/master/screenshots/viewpager.gif" width="190" height="270" />

## Installation

Add the dependency to your module build.gradle:
```java
dependencies {
	        implementation 'in.dd4you.animatoo:anim:1.0.0'
}
```
## Usage
### DDAnimatoo has 15 different activity/Fragment transition animations:

01. in and out.
02. swipe left.
03. swipe right.
04. split.
05. shrink.
06. card.
07. zoom.
08. fade.
09. spin.
10. diagonal.
11. windmill.
12. slide up.
13. slide down.
14. slide left.
15. slide right.

### DDAnimatoo has 12 different ViewPager/ViewPager2 transition animations:

01. Background To Foreground.
02. Cube In.
03. Cube Out.
04. Depth Page.
05. Flip Horizontal.
06. Flip Vertical.
07. Foreground To Background.
08. Rotate Down.
09. Rotate Up.
10. Tablet Page.
11. Zoom In.
12. Zoom Out.

## For Activity
Using DDAnimatoo is extremely simple, A single short line of code following startActivity(...) is all that's needed, for example:
```java
startActivity(new Intent(context, TargetActivity.class));
Animatoo.animateZoom(context);  //fire the zoom animation
```
Another example, this time firing the animation when the back button is pressed:
```java
@Override
public void onBackPressed(){
  super.onBackPressed();
  Animatoo.animateSlideLeft(context); //fire the slide left animation
}
```
## For Fragment
Using DDAnimatoo is extremely simple, A single short line of code following FragmentTransaction(...) is all that's needed, for example:
```java
FragmentTransaction fragmentTransaction = getSupportFragmentManager().beginTransaction();
FrAnimatoo.animateZoom(fragmentTransaction);  //fire the zoom animation
fragmentTransaction.replace(frameLayout.getId(), new FragmentName());
fragmentTransaction.commit();
```


## For ViewPager
Using DDAnimatoo is extremely simple, A single short line of code, for example:
```java
viewPager.setPageTransformer(new VpAnimatoo.BackgroundToForeground())
```

## For ViewPager2
Using DDAnimatoo is extremely simple, A single short line of code, for example:
```java
viewPager2.setPageTransformer(new Vp2Animatoo.BackgroundToForeground())
```


## All the available methods for Activity:
```java
Animatoo.animateZoom(context);
Animatoo.animateFade(context);
Animatoo.animateWindmill(context);
Animatoo.animateSpin(context);
Animatoo.animateDiagonal(context);
Animatoo.animateSplit(context);
Animatoo.animateShrink(context);
Animatoo.animateCard(context);
Animatoo.animateInAndOut(context);
Animatoo.animateSwipeLeft(context);
Animatoo.animateSwipeRight(context);
Animatoo.animateSlideLeft(context);
Animatoo.animateSlideRight(context);
Animatoo.animateSlideDown(context);
Animatoo.animateSlideUp(context);
```


## All the available methods for Fragment:
```java
FrAnimatoo.animateZoom(fragmentTransaction);
FrAnimatoo.animateFade(fragmentTransaction);
FrAnimatoo.animateWindmill(fragmentTransaction);
FrAnimatoo.animateSpin(fragmentTransaction);
FrAnimatoo.animateDiagonal(fragmentTransaction);
FrAnimatoo.animateSplit(fragmentTransaction);
FrAnimatoo.animateShrink(fragmentTransaction);
FrAnimatoo.animateCard(fragmentTransaction);
FrAnimatoo.animateInAndOut(fragmentTransaction);
FrAnimatoo.animateSwipeLeft(fragmentTransaction);
FrAnimatoo.animateSwipeRight(fragmentTransaction);
FrAnimatoo.animateSlideLeft(fragmentTransaction);
FrAnimatoo.animateSlideRight(fragmentTransaction);
FrAnimatoo.animateSlideDown(fragmentTransaction);
FrAnimatoo.animateSlideUp(fragmentTransaction);
```


## All the available methods for ViewPager:
```java
new VpAnimatoo.BackgroundToForeground()
new VpAnimatoo.CubeIn()
new VpAnimatoo.CubeOut()
new VpAnimatoo.DepthPage()
new VpAnimatoo.FlipHorizontal()
new VpAnimatoo.FlipVertical()
new VpAnimatoo.ForegroundToBackground()
new VpAnimatoo.RotateDown()
new VpAnimatoo.RotateUp()
new VpAnimatoo.TabletPage()
new VpAnimatoo.ZoomIn()
new VpAnimatoo.ZoomOut()
```

## All the available methods for ViewPager2:
```java
new Vp2Animatoo.BackgroundToForeground()
new Vp2Animatoo.CubeIn()
new Vp2Animatoo.CubeOut()
new Vp2Animatoo.DepthPage()
new Vp2Animatoo.FlipHorizontal()
new Vp2Animatoo.FlipVertical()
new Vp2Animatoo.ForegroundToBackground()
new Vp2Animatoo.RotateDown()
new Vp2Animatoo.RotateUp()
new Vp2Animatoo.TabletPage()
new Vp2Animatoo.ZoomIn()
new Vp2Animatoo.ZoomOut()
```


# Contribution


Please fork repository and contribute using pull requests.

Any contributions, large or small, major features, bug fixes, additional language translations, unit/integration tests are welcomed and appreciated but will be thoroughly reviewed and discussed.



# License

    Copyright 2020 DD4You.in

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

