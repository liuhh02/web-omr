# web-omr
Web-based Optical Music Recognition tool that translates musical notes on monophonic scores to ABC notation and annotates the ABC notes onto the music score to facilitate the process of learning music.

This project was created in a 2 day hackathon at [YouthHacks 2019](https://youthhacks.org/). 

## Getting Started
This web app is developed with Flask on a [tensorflow model](https://github.com/calvozaragoza/tf-deep-omr) built by Calvo-Zaragoza et al. published as [End-to-End Neural Optical Music Recognition of Monophonic Scores](https://www.mdpi.com/2076-3417/8/4/606) in the Applied Sciences Journal 2018.
To get started, follow the steps below:

 1. Install the relevant dependencies: tensorflow v1, flask
 2. Download the [semantic model](https://grfia.dlsi.ua.es/primus/models/PrIMuS/Semantic-Model.zip) developed by Calvo-Zaragoza et al.
 3. Download the [semantic vocabulary](https://github.com/calvozaragoza/tf-deep-omr/blob/master/Data/vocabulary_semantic.txt)
 4. Download the font [Aaargh.ttf](https://www.fontsquirrel.com/fonts/aaargh) (this is needed to annotate the image with the ABC notation)
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE5MTk2ODI0MCwtMTIxNTA4ODk2Ml19
-->