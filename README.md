# jquery-smooth-scroll-to-section

## #1
```
jQuery('.nav-link').on('click', function (event) {
        event.preventDefault();
        var element = jQuery(this.hash);
        jQuery('html,body').animate({ scrollTop: element.offset().top },);
    });
```    
## #2
```
jQuery('.nav-link').on('click', function (event) {
        event.preventDefault();
        var element = jQuery(this.hash);
        jQuery('html,body').animate({ scrollTop: element.offset().top },2000);
    });
```    
## #3
```
jQuery('.nav-link').on('click', function (event) {
        event.preventDefault();
        var element = jQuery(this.hash);
        jQuery('html,body').animate({ scrollTop: element.offset().top },'normal', 'swing');
    });    
```
## #4
```
jQuery('a[href*=#]:not([href=#])').on('click', function (event) {
        event.preventDefault();
        var element = jQuery(this.hash);
        jQuery('html,body').animate({ scrollTop: element.offset().top },'normal', 'swing');
    });
```    
## #5 
```
  jQuery('a[href*=#]:not([href=#])').on('click', function (event) {
        event.preventDefault();
        var element = jQuery(this.hash);
        jQuery('html,body').animate({ scrollTop: element.offset().top - 200},);
    });
```    
## #6 (Best)
```
jQuery('a[href*=#]:not([href=#])').on('click', function (event) {
        event.preventDefault();
        var element = jQuery(this.hash);
          var headerheight  =jQuery("header").outerHeight(true);
        jQuery('html,body').animate({ scrollTop: element.offset().top - headerheight},);
    });
```    
