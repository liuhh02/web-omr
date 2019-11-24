# web-omr
Web-based Optical Music Recognition tool that translates musical notes on monophonic scores to ABC notation and annotates the ABC notes onto the music score to facilitate the process of learning music.
![Sample Result](https://imgur.com/Dl1HYS2)
This project was created in a 2 day hackathon at [YouthHacks 2019](https://youthhacks.org/). 

## Getting Started
This web app is developed with Flask on a [tensorflow model](https://github.com/calvozaragoza/tf-deep-omr) built by Calvo-Zaragoza et al. published as [End-to-End Neural Optical Music Recognition of Monophonic Scores](https://www.mdpi.com/2076-3417/8/4/606) in the Applied Sciences Journal 2018.
To get started, follow the steps below:

 1. Install the following dependencies: tensorflow v1, flask
 2. Download the [semantic model](https://grfia.dlsi.ua.es/primus/models/PrIMuS/Semantic-Model.zip) developed by Calvo-Zaragoza et al.
 3. Download the [semantic vocabulary](https://github.com/calvozaragoza/tf-deep-omr/blob/master/Data/vocabulary_semantic.txt)
 4. Download the font [Aaargh.ttf](https://www.fontsquirrel.com/fonts/aaargh) (this is needed to annotate the image with the ABC notation)

If you would like to train the semantic model yourself, head over to the tensorflow model [Github repository](https://github.com/calvozaragoza/tf-deep-omr) for instructions and download the [PrIMuS dataset](https://grfia.dlsi.ua.es/primus/).

Make sure your folder structure is as follows:
```
app.py
vocabulary_semantic.txt
Aaargh.ttf
├── Semantic-Model
|   ├── semantic_model.meta
|   └── semantic_model.index
|   └── semantic_model.data-00000-of-00001
├── templates
|   ├── index.html
|   └── result.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2007-10-29-why-every-programmer-should-play-nethack.textile
|   └── 2009-04-26-barcamp-boston-4-roundup.textile
├── _data
|   └── members.yml
├── _site
└── index.html
```
app.py
vocabulary_semantic.txt

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTEzOTE2Njg1NiwtMTk1MzE0MDE3NSwtMT
IxNTA4ODk2Ml19
-->