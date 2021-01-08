## Youtube-Video-Info-Scraper
A python library that uses browser automation to scrape video details of any youtube video including views, likes, dislikes, comments,published date, channel link etc.
It uses [datakund](https://pypi.org/project/datakund) internally

Complete Documentation available [here](https://youtube-api.datakund.com/en/latest/)


### Support
For any help / feedback you can message us here
* datakund@gmail.com
* https://t.me/datakund

### Installation

```sh
pip install youtube-video-scraper
```

### Import

```javascript
from youtube-video-scraper import *
```

### Fetch Video Details

To fetch title, description, likes, comments,dislikes,duration,subscribers etc. of youtube video we use ``get_video_info`` method.
It requires **video_url** as input parameter

```javascript
response=youtube.get_video_info(video_url="video_url_here")
video_details=response['body']
```

### Example Response

```sh
{
   "DisLikes":"DisLikes",
   "Title":"Title",
   "Subscribers":"Subscribers",
   "Comments":"Comments",
   "ChannelLink":"ChannelLink",
   "ChannelName":"ChannelName",
   "Desc":"Desc",
   "Views":"Views",
   "Duration":"Duration",
   "Publish_Date":"Publish_Date",
   "Likes":"Likes"
}
...
```

### DataKund
It uses [datakund](https://pypi.org/project/datakund/) internally to do browser automation
DataKund is an automation library that uses selenium & supports automation of many sites including [Youtube](https://youtube-api.datakund.com/en/latest/), [Amazon](https://amazon-api.datakund.com/en/latest/), [Twitter](https://twitter-api.datakund.com/en/latest/), [LinkedIn](https://linkedin-api.datakund.com/en/latest/) , [Google](https://google-api.datakund.com/en/latest/) etc.
