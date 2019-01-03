### python-pixabay
Python 2 & 3 Pixabay's API wrapper.

### Install from PyPi
`pip install python-pixabay`

### Synopsis

```python
from pixabay import Image, Video

api_key = 'my_pixabay_api_key'

# ***************
# * Image/Photo *
# ***************
image = Image(api_key)

# default image search
image.search()

# custom image search
image.search(q='cats dogs',
             lang='es',
             response_group='high_resolution',
             image_type='photo',
             orientation='horizontal',
             category='animals',
             safesearch='true',
             order='latest',
             page=2,
             per_page=3)

# *********
# * Video *
# *********

video = Video(api_key)

# default video search
video.search()


# custom video search
video.search(q='cats', lang='fr',
                       video_type='animation',
                       category='animals',
                       page=1,
                       per_page=4)
```

### How do I use it?

I wrote a few _how to_ articles in the [project wiki](https://github.com/momozor/python-pixabay/wiki). Feel free to add more examples or scenarios to the wiki.

### Running the test

> Make sure you set PIXABAY_KEY environment variable with your pixabay api key assigned before running the command below

* Via Python unittest's discover: `python -m unittest discover test`

* or via nose: `nosetests`

### SEE ALSO
[Pixabay API documentations](https://pixabay.com/api/docs)

### LICENSE

This module is licensed under the MIT license. See LICENSE file for more details.

### AUTHOR

* momozor <skelic3@gmail.com>
