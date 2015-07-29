# Website Performance Optimization portfolio project

## Index.html – Optimization Tasks

* Ran index.html through Google PageSpeed – 54/100 (mobile)
60/100 (desktop)

* Added async attribute to analytics.js <script> tag so that
it doesn’t block DOM processing – 54/100 (mobile) 61/100 (desktop)

* Added media attributes to CSS stylesheet – 54/100 (mobile)
61/100 (desktop)

* Compressed/optimized images with Imagemagick cli – 75/100
(mobile) 88/100 (desktop)

* Minified CSS/JS – 75/100 (mobile) 88/100 (desktop)

* Removed Google Font and use sans-serif instead – 84/100
(mobile) 91/100 (desktop)

* Inline CSS for screen - 95/100 (mobile) 91/100 (desktop)

## Pizza.html – Optimization tasks (fixed forced sync layout issues)

* Cached Math.sin calculation outside the for loop in
updatePositions(); to achieve 60 fps (reduced average time to load
last 10 frames from 40ms to 2ms – a 95% decrease in load time)

* Cached querySelectorAll() and simplified newWidth
calculation in changePizzaSizes(); (reduced time to resize pizzas
from 160ms to 0.5ms – a 99.69% decrease in load time)

* Replaced getElementsByClassName() instead of querySelectorAll() to 
improve performance (reverted - see inline comments - line 441)

* Use screen height to calculate number of pizzas to display rather than 
having it hard coded to 200 pizzas (see inline comments - line 521)


## To run:

1. Check out the repository
1. Start a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080