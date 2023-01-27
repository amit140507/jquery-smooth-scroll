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
