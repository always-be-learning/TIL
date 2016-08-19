# Creating `Date` objects in multiple browsers

Today, I'm working on a code challenge and part of the challenge involves dates (finding a range of them, stashing them in an object, etc.). I've done the bulk of my development in Chrome & its inspector and console and as of now (August 2016) I'm new enough to writing Javascript on my own that I'm not yet fluent in browser differences w/r/t javascript.

You can see where this is going, right?

I turned in the challenge and heard back that it has "significant bugs". Hmph. After I spent a little time being cranky and incredulous, I did what a frontend developer does: I opened up more browsers. And boom! Firefox and Safari go on and on about how my dates are `NaN/Nan`. 

_Ugh_

A very little bit of searching taught me that Firefox and Safari don't much care for Date objects with dashes, they want forward slashes instead, thanks very much.

:confounded:

Happily, I found the tiniest of fixes at StackOverflow: http://stackoverflow.com/a/21984717

```javascript
  // the dates in the challenge JSON files look like this:
  // "2013-04-16 07:20:32"

  // instead of just going straight to new date objects like this:
  start = new Date(start_date);
  end = new Date(end_date);

  // now, I swap in the slashes and _then_ make new objects:
  start_date = start_date.replace(/-/g,'/');
  end_date = end_date.replace(/-/g,'/');
  start = new Date(start_date);
  end = new Date(end_date);  
```

And now my UI shows actual dates instead of `Nan/Nan`. :tada: