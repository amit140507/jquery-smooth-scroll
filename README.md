# jquery-smooth-scroll

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
