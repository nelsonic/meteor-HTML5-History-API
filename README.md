# Meteor HTML5 History API

If your Meteor app/site uses routes (e.g: [IronRouter][]) and
needs to run in an older browser (pre-HTML5) 
you will need a [Polyfill][] for [HTML5 History][].

This package loads a file called **history.js** into your app 
giving older browsers the [HTML5 History API][] 


## Install

```
mrt add HTML5-History-API
```

- - - 

## Background on HTML5 History

Modern ("Single Page") Web Apps change the url in the browser
and display fresh content without refreshing the page.

In order to *remember* which pages have been visited 
(and thus be able to use the browser's back/forward button) the 
[HTML5 History][] was added in 

Demos: http://html5demos.com/history

### Internet Explorer!

Sadly, 20% of internet users are still stuck on Internet Explorer pre v.10
(and older versions of both IOS and Android's *stock* browsers do not support
HTML5 History) so in order to give these visitors the single-page-app 
experience you need to include this package.

![Can I Use - History](http://i.imgur.com/5RNZBG9.png)

See: http://caniuse.com/#search=history


[IronRouter]: https://github.com/EventedMind/iron-router
[Polyfill]: http://remysharp.com/2010/10/08/what-is-a-polyfill
[HTML5 History]: http://html5doctor.com/history-api/
[HTML5 History API]: https://github.com/devote/HTML5-History-API