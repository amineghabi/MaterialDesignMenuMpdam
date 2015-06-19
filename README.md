# GhabiMD animation

New library, that provides a simple way to implement Material design styled Menu animation for your apps.



there is a screenshot for this styled Menu animation.

<img src="https://d13yacurqjgara.cloudfront.net/users/495792/screenshots/2018249/draft_06.gif" alt="Guillotine animation gif" style="width:800;height:600">


# Usage

*For a working implementation, have a look at the app module*

1. Include the library as local library project.

2. Your hamburger on navigation menu must have exactly same coordinates as hamburger on ActionBar.

3. In your `onCreate` method you need to config and build animation with GuillotineAnimation.GuillotineBuilder

	```java
    new AndrogeekAnimation.GuillotineBuilder(guillotineMenu, guillotineMenu.findViewById(R.id.guillotine_hamburger), contentHamburger)
                .setActionBarViewForAnimation(toolbar)
                .build();
     ```
Here `setActionBarViewForAnimation` method enables bounce effect of ActionBar at the end of the guillotine closing animation.

# Misc

Builder allows you to customize start delay, duration, interpolation and you can set listener if you want to do staff at the moment when menu has been opened or closed.

# Compatibility
  
  * Android 4.0.3 Ice Cream Sandwich (API level 15)
  
# Changelog

### Version: 1.0

  * Initial Build
  
## License

    Copyright 2015, MPDAM ISETR .
