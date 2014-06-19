##  Content Strategy

With the theme of masonry as a front end layout, we coupled the "brick" content type.

Bricks have sizes (1x1, 2x2, 4x1, etc.) and types (content, slideshow, image, etc.), defined via field UI. We send that info in the JSON to tell Angular how to render them.

A page is made up of many bricks... Bricks are placed in per page Nodequeues to handle inclusion and order.

Views pulls in the bricks using Nodequeue as a filter/sort and provides their details in JSON streams.

Angular consumes the JSON and does frontendy things to render it all pretty like.