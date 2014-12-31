# History #

+ Initial project was done by [Juan S. Escobar](https://github.com/escobar5/raphael-pan-zoom)
+ [Daan Poron](https://github.com/daanporon/raphael-pan-zoom) has added some improvements as touchevent
+ This fork have purpose to be integrate on previous project, waiting pull request validation

# Documentation #

## Minial usage ##

    <script type="text/javascript" src="js/raphael-min.js"></script>
    <script type="text/javascript" src="js/hammer.min.js"></script>
    <script type="text/javascript" src="js/raphael.pan-zoom.js"></script>
    
    <script type="text/javascript">

    	$(document).ready(function(){    	    
            var r = Raphael('mapsvg',500,500);
            var panZoom = r.panzoom();
            panZoom.enable();
        });
    </script>
    
## Options ##

### zoomStep ###

+ default : 0.1

### maxZoom ###

+ type number
+ default : (1 / settings.zoomStep)

### minZoom ###

+ type number
+ default : 0

### initialZoom ###

+ type number
+ default : 0

### initialPosition ###

+ default : { x: 0, y: 0 }
    
### gestures ###

+ default : false

### onPan ###

+ default : null

### onZoom ###

+ default : null

### onRepaint(currZoom) ###

Called when repaint() happens in pan-zoom.

+ default : null

### panLimit ###

+ default : true
