jquery.forwardevents
====================

jQuery plugin which forwards mouse events from one DOM Element to another.

Based on the jQuery code from http://e-infotainment.com/applications/jquery-plugins/behaviours/forward-mouse-events/


Usage:

1. Include the js file after jQuery itself.

2. In your document ready code:

  $('.mask').forwardevents();

This will forward all of $('.mask')'s events to the element directly underneath. It does this by rapidly hiding and showing .mask, so it may or may not be suitable for your purposes.

To get around this, there is another mode which allows you to bypass the detection and send events directly to a certain element:

$('.mask').forwardevents( {directEventsTo:$('.underlyingdiv')} );

This should forward all events to .underlyingdiv only and skip the detection step.
