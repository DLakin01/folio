---
layout: post
title: Bloc Jams
image: ../images/bloc_jams_bg.jpeg
---

___Technologies used: AngularJS, CSS3, JavaScript, jQuery, Buzz, and others___

**About the Project**

Bloc Jams is a compact, light-weight music player built in Angular, using jQuery, vanilla JavaScript, and several outside libraries to offer fun listening experience to users. This project featured my first in-depth use of the Angular framework, which I immediately took to. I had an intuitive feel for the modularity and elegance of the Model-View-Controller framework, and used that to break out the functions of a music player across the breadth of an Angular app.

<div class="img_row squish">
  <img class="col three" src="{{ site.baseurl }}/images/blocjams_example.jpeg">
</div>

In building Bloc Jams, I did hit some stumbling blocks. In particular, for a time the various links on the Collection Page all pointed to the same place, even if they referred to different albums. I got around that issue by making use of URL queries and the QueryData library. By inserting readable information into the URLs of the various links, I was able to use the QueryData information to tell the rest of the code which album to load. Some of the relevant code is on display below:

{% highlight javascript %}
var albumPicker = function() {
  var queryData = new QueryData;
  if(queryData.albumID === '1') {
    setCurrentAlbum(albumBonIver);
  }
  else if(queryData.albumID === '2') {
    setCurrentAlbum(albumFooFighters);
  }
  else if(queryData.albumID === '3') {
    setCurrentAlbum(albumSufjan);
  }
};
{% endhighlight %}


You can check out Bloc Jams and listen to some good tunes [here.](https://bloc-jammr.herokuapp.com) Happy listening!

[GitHub repo](https://github.com/dlakin01/bloc-jams-angularjs)
