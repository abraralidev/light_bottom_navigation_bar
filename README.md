# [light_bottom_navigation_bar](https://pub.dev/packages/light_bottom_navigation_bar/install)
## current version: 0.0.1

Amazing powerful animated widget, it is useful for modern apps by displaying pro BottomNavigationBar with ViewPager.

Add Super BottomNavigationBar => Better UI/UX.

Do you like circles ? see  [super_circle](https://pub.dev/packages/super_circle)


[![pub](https://img.shields.io/pub/v/light_bottom_navigation_bar?color=blue&label=pub&logo=flutter&style=flat-square)](https://pub.dev/packages/light_bottom_navigation_bar/install)
[![license](https://img.shields.io/github/license/abraralidev/light_bottom_navigation_bar?color=yellow&label=license&logo=github&style=flat-square)](https://pub.dev/packages/light_bottom_navigation_bar/install)
[![repo_size](https://img.shields.io/github/languages/code-size/abraralidev/light_bottom_navigation_bar?color=red&label=repo_size&logo=github&style=flat-square)](https://pub.dev/packages/light_bottom_navigation_bar/install)



<div align="center">
<img src="https://github.com/abraralidev/light_bottom_navigation_bar/raw/main/screenshots/gifs/demo.gif" width="30%" height="30%" alt="demo"/>
<img src="https://github.com/abraralidev/light_bottom_navigation_bar/raw/main/screenshots/images/img4.jpg" width="30%" height="30%" alt="photo"/>
</div>



# Features

**Animation**

You can feel the animation with this package when tab is selected.

**Configurable Widget**

You can control any part of this widget backgroundColor , icons , size , type of animation , colors and more...

**Strong build**

The package is built with strong tests to make it trusted to developers

**Beautiful UI**

With this package you can make `POWERFUL` UI.



# Installing

Add this to your package's `pubspec.yaml` file:

```yaml
dependencies:
  light_bottom_navigation_bar: latest_version
```

Then import it :

```dart
import 'package:light_bottom_navigation_bar/light_bottom_navigation_bar.dart';
```

More details see [pub.dev](https://pub.dev/packages/light_bottom_navigation_bar/install).



# Usage

The `light_bottom_navigation_bar` package you can use it simply :



> :warning:: The `items` value must be `items >= 1`.


> :warning:: The `currentIndex` value must be `currentIndex >= 0 && currentIndex < items.length`.



**Simple Design**

```
      Scaffold(
              bottomNavigationBar: LightBottomNavigationBar(
                currentIndex: 1,
                items: [
                  LightBottomNavigationBarItem(),
                  LightBottomNavigationBarItem(),
                  LightBottomNavigationBarItem(),
                ],
                onSelected: (index){
                  print('tab $index');
                },
              ),
      ...........
          );
```


<div align="center">
<img src="https://github.com/abraralidev/light_bottom_navigation_bar/raw/main/screenshots/images/img1.jpg" width="300" alt="simple_design"/>
</div>



**Normal Design**

```
      Color primaryColor = Colors.yellowAccent;
      ........
      Scaffold(
              bottomNavigationBar: LightBottomNavigationBar(
                currentIndex: 1,
                items: [
                  LightBottomNavigationBarItem(
                    unSelectedIcon: Icons.home_outlined,
                    selectedIcon: Icons.home,
                    splashColor: primaryColor,
                    borderBottomColor: primaryColor,
                    backgroundShadowColor: primaryColor,
                    selectedIconColor: primaryColor,
                    unSelectedIconColor: Colors.grey
                  ),
                  LightBottomNavigationBarItem(
                      unSelectedIcon: Icons.favorite_border,
                      selectedIcon: Icons.favorite,
                      splashColor: primaryColor,
                      borderBottomColor: primaryColor,
                      backgroundShadowColor: primaryColor,
                      selectedIconColor: primaryColor,
                      unSelectedIconColor: Colors.grey
                  ),
                  LightBottomNavigationBarItem(
                      unSelectedIcon: Icons.cloud_done_outlined,
                      selectedIcon: Icons.cloud_done,
                      splashColor: primaryColor,
                      borderBottomColor: primaryColor,
                      backgroundShadowColor: primaryColor,
                      selectedIconColor: primaryColor,
                      unSelectedIconColor: Colors.grey
                  ),
                ],
                onSelected: (index){
                  print('tab $index');
                },
              ),
          ...........
           );
      
```


<div align="center">
<img src="https://github.com/abraralidev/light_bottom_navigation_bar/raw/main/screenshots/images/img2.jpg" width="300" alt="normal_design"/>
</div>



**Super Design**

```
      Scaffold(
              bottomNavigationBar: LightBottomNavigationBar(
                currentIndex: 2,
                items: makeNavItems(),
                onSelected: (index){
                  print('tab $index');
                },
              ),
         .........
          );
      
      
      List<LightBottomNavigationBarItem> makeNavItems() {
         return [
               LightBottomNavigationBarItem(
                 unSelectedIcon: Icons.home_outlined,
                 selectedIcon: Icons.home_outlined,
                 size: 30,
                 backgroundShadowColor: Colors.red,
                 borderBottomColor: Colors.red,
                 borderBottomWidth: 3,
                 // highlightColor: Colors.red,
                 // hoverColor: ,
                 splashColor: Colors.red,
                 selectedIconColor: Colors.red,
                 unSelectedIconColor: Colors.red
               ),
               LightBottomNavigationBarItem(
                   unSelectedIcon: Icons.search_outlined,
                   selectedIcon: Icons.search_outlined,
                   size: 30,
                   backgroundShadowColor: Colors.blue,
                   borderBottomColor: Colors.blue,
                   borderBottomWidth: 3,
                   // highlightColor: Colors.red,
                   // hoverColor: ,
                   splashColor: Colors.blue,
                   selectedIconColor: Colors.blue,
                   unSelectedIconColor: Colors.blue
               ),
               LightBottomNavigationBarItem(
                   unSelectedIcon: Icons.star_border_outlined,
                   selectedIcon: Icons.star_border_outlined,
                   size: 30,
                   backgroundShadowColor: Colors.yellowAccent,
                   borderBottomColor: Colors.yellowAccent,
                   borderBottomWidth: 3,
                   // highlightColor: Colors.red,
                   // hoverColor: ,
                   splashColor: Colors.yellowAccent,
                   selectedIconColor: Colors.yellowAccent,
                   unSelectedIconColor: Colors.yellowAccent
               ),
               LightBottomNavigationBarItem(
                   unSelectedIcon: Icons.done_outline_rounded,
                   selectedIcon: Icons.done_outline_rounded,
                   size: 30,
                   backgroundShadowColor: Colors.green,
                   borderBottomColor: Colors.green,
                   borderBottomWidth: 3,
                   // highlightColor: Colors.red,
                   // hoverColor: ,
                   splashColor: Colors.green,
                   selectedIconColor: Colors.green,
                   unSelectedIconColor: Colors.green
               ),
               LightBottomNavigationBarItem(
                   unSelectedIcon: Icons.person_outline,
                   selectedIcon: Icons.person_outline,
                   size: 30,
                   backgroundShadowColor: Colors.purpleAccent,
                   borderBottomColor: Colors.purpleAccent,
                   borderBottomWidth: 3,
                   // highlightColor: Colors.red,
                   // hoverColor: ,
                   splashColor: Colors.purpleAccent,
                   selectedIconColor: Colors.purpleAccent,
                   unSelectedIconColor: Colors.purpleAccent
               ),
             ];
      }
```


<div align="center">
<img src="https://github.com/abraralidev/light_bottom_navigation_bar/raw/main/screenshots/images/img3.jpg" width="300" alt="super_design"/>
</div>



# Widget Properties

**LightBottomNavigationBar**


`items`

*List<LightBottomNavigationBarItem>  (required)*

list of LightBottomNavigationBarItem to show them in your BottomNavigationBar.



`currentIndex`

*int*

The tab to display.



`height`

*double*

Height of the BottomNavigationBar.



`backgroundColor`

*Color*

backgroundColor of BottomNavigationBar.



`curve`

*Curve*

The transition curve.



`duration`

*Duration*

The transition duration.
 
 
 
`padding`
 
 *EdgeInsets*
 
The padding surrounding the entire widget , You can use to adding floating effect.



`elevation`
 
 *double*
 
The elevation of the widget.



`onSelected`
 
 *ValueChanged<int>?*
 
Callback method , Return the index of the tab that was tapping.


---

