# DDAnimatoo

[ ![Download](https://api.bintray.com/packages/dd4you/DD4YouAppsConfig/in.dd4you.animatoo/images/download.svg) ](https://bintray.com/dd4you/DD4YouAppsConfig/in.dd4you.animatoo/_latestVersion)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg?style=flat-square)](https://www.apache.org/licenses/LICENSE-2.0.html)


Bored with same animation for activity, Fragment, ViewPager and Viewpager2 transition? DDAnimatoo is a lightweight and easy to use Android library that provides many activity, Fragment, ViewPager and Viewpager2 transition animations.
* min SDK 16 (Android Jellybean 4.1)
* written in Java

A lightweight, easy-to-use Android library that provides awesome activity, Fragment, ViewPager and Viewpager2 transition animations


## Screenshots
<img src="https://github.com/mohammadatif/Animatoo/blob/master/Screen%20Shots/Card.gif" width="190" height="270" />
<img src="https://github.com/mohammadatif/Animatoo/blob/master/Screen%20Shots/Diagonal.gif" width="190" height="270" />

## Installation

Add the dependency to your module build.gradle:
```java
dependencies {
	        implementation 'in.dd4you.animatoo:anim:1.0.0'
}
```
## Usage
DDAnimatoo has 15 different activity and Fragment transition animations:

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


## All the available methods for this library:
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

# Inspiration

This library was made by possible based on code and design inspiration from these sources:  
https://github.com/AtifSayings/Animatoo


# Contribution


Please fork repository and contribute using pull requests.

Any contributions, large or small, major features, bug fixes, additional language translations, unit/integration tests are welcomed and appreciated but will be thoroughly reviewed and discussed.
