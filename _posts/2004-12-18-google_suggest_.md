---
layout: single
title: "Google Suggest Dissected"
slug: "Google Suggest Dissected"
redirect_from:
  - /2004/12/google_suggest_.html
  - /2004/12/google_suggest_/
date:   2004-12-18 08:44:31 -0700
# image:  logo_google_suggest.gif
tags: 
  - User Interface
  - Google
  - Javascript
  - Web/Tech

categories:
  - ephemera
class:
  - wide

excerpt_seperator: <!--more-->
permalink: /ephemera/google-suggest-dissected/
---

As a former Macintosh developer, I've always been disappointed with the user-interface of web pages. The state of the art of UI design moved backwards with the advent of the browser -- we traded connectivity for ease-of-use. With the advent of pages written in Flash, some better user-interfaces were created, but at the important cost of things like being able to copy text, have semantic and meta-data information imbedded in web pages, searchability, etc.

So I keep an eye out for innovative ideas that preserve the essence of what is so powerful about web pages, yet also offer a good ideas. My posts on [Map Mashup](/2004/10/map_mashup.html) and [TiddlyWiki](/2004/09/tiddlywiki.html) offer some interesting web UI exemplars.

<a href="https://web.archive.org/web/20051124093032/http://www.google.com/webhp?hl=en&complete=1"><a href="#"><img width="230px" style=" margin-right:15px" align="right"  src="{{ site.url }}{{ site.baseurl }}/assets/images/logo_google_suggest.gif" alt="logo_google_suggest"/></a></a>

To this list of exemplars I now add [Google Suggest](http://www.google.com/webhp?hl=en&complete=1) by Google programmer [Kevin Gibbs](http://www.google.com/googleblog/2004/12/ive-got-suggestion.html), who wrote this as part of Google employee's ability to work 20% of the time on their own projects. Google Suggest replaces the browser's default auto-complete with one specific to Google searching. As you type each letter of your search request, you are shown the most popular requests for that term, and how many search hits are available for that search term. You really have to try out to understand how amazing and intuitive it is.

Blogger [Chris Justus](http://serversideguy.blogspot.com/) has [dissected and documented](http://serversideguy.blogspot.com/2004/12/google-suggest-dissected.html) how Google Suggest works. If you are a web developer, I recommend you read his analysis and I hope it will inspire you.

This specific technique is probably not useful for all web sites -- the amount of load that even a small number of users can place on a database using this technique requires a large server infrastructure, as basically every time you type a letter a database is being hit. Google can do this as they understand server farms and how to scale large loads. However, as inspiration for other ideas, I think it is marvelous.

For instance, I didn't know you could take control over your browsers auto-complete functionality by setting autocomplete="off" in your input field. Given this and the other techniques for display and cursor control, you could create dynamic auto-complete functionality on your own web pages, but skip the bandwidth intensive XMLHttpRequest by either caching the data in your web page, or in a user's cookie, or both. An example of this is [BitFlux](http://blog.bitflux.ch/) blog's [LiveSearch](http://blog.bitflux.ch/archive/livesearch_roundup.html) functionality (which is also documented [here](http://blog4.bitflux.ch/wiki/LiveSearch)).

The technique for retrieving the data using XMLHttpRequest is also marvelous. This functionality has been [around for a while](http://developer.apple.com/internet/webcontent/xmlhttpreq.html) but this is one of the cleanest examples of how to do it on the client side.

I've got some other ideas on how to apply some of these techniques to Wiki pages -- hopefully in the next few months I'll have some proof-of-concept examples for you to play around with.

In addition, Google Suggest is now, in a sense, a new web service from google that can be used independently. For instance Adam Stiles has [written](http://www.adamstiles.com/adam/2004/12/hacking_google_.html) about a [hack](http://www.netcaptor.net/adsense/suggest.php) to help suggest keywords for AdSense.

### Comments

Google Suggest is definitely interesting, and Kevin Gibbs is to be congratulated for putting it together. It's an elegant piece of work. I think the most intersting things, though, aren't about the ability to use RPC calls from Javascript. This is pretty old stuff. Brent Ashley released the JSRS library (http://www.ashleyit.com/rs/main.htm) some years ago (cf. these two articles at IBM from 2001: http://www-106.ibm.com/developerworks/library/wa-resc/?dwzone=web, http://www-128.ibm.com/developerworks/web/library/wa-rich/). The technique is somewhat different, using a hidden Iframe as a buffer, but the effect is the same. On the technical side, making this workable in real time is impressive. Rather than triggering actions with they onkeypress event, the input field is checked periodically with a timer. This means you don't have to wait from a response from google when you type something - if you get three letters entered in between checks, it will still appear nearly instant. (The above referenced article by Chris Justus may cover this, I can't recall at the moment). And the server side stuff required to be able to return search result counts so quickly has to be very well put together. On the non-developer side, what I find intersting is that something that has been possible for over three years is hitting the mainstream because Google's done it. There are tremendous boosts in usability possible using RPC calls, but in my somewhere over six years of web consulting, usability has always been the hardest sell. Now that there's a high profile application of this technique, I expect it will become as popular as CNET's orange menu bar was. (If only they had put that on the right side...).

[dwayne](http://iconys.com) 2004-12-21T17:56:03-07:00

dwayne's exactly right - interest in Javascript RPC has increased exponentially since GMail and now Google Suggest. I've seen hits to my remote scripting pages go crazy, with the side effect that my referrer spam has spiralled as well. I first started building rich UIs with MS Remote Scripting in 1998, and I haven't done any development on JSRS for a couple of years now. If I had the time or inclination to redo it now, I would definitely use XMLHTTP. I had to use iframe/layer at the time for wide compatibility. The image/cookie method is a great one for smaller stuff - I use ut to great effect at http://www.blogchat.com

[Brent Ashley](http://www.ashleyit.com/rs) 2005-01-04T11:20:28-07:00

If you like Google Suggest you will love this french tool called Pertimm. Take a look at this technology. It's really worth it. in order to access to a demo contact them at : http://www.pertimm.com/en/contact/index.htm

[Pierre Vesoul](http://pouncha.typepad.com) 2005-02-22T07:35:30-07:00

You might appreciate my "Zuggest" tool. It uses "Ajax" concepts and works similarly to Google Suggest but searches against the Amazon Product database as you're typing. Check it out: http://www.FrancisShanahan.com/zuggest.aspx It's built with Javascript, Amazon Web Services, SOAP, XMLHttp, XML, C# and ASP.NET and SQL Server. Would love to get some feedback on it. -fs

[Francis](http://www.FrancisShanahan.com) 2005-03-04T19:21:34-07:00

I noticed that google suggest does not show same number of results as google.com itself: http://www.nirendra.net/cms/google/suggest -Nirendra

[Nirendra Awasthi](http://www.nirendra.net) 2005-05-11T13:38:36-07:00

This is another case where people are astonished to learn that there isn't any black magic going on here and that the functionality is there. it just takes quite a lot of fiddling to get right and in a form that is reusable. This is why I think that there is still a component market for these kinds of things. the google suggest and gmail suggest functionality has been commercialized already here: http://developer.ebusiness-apps.com/technologies/webdevelopment/codeandcomponents/ebawebcombov3/media/demos.htm

[alexei](http://www.alexeiwhite.com) 2005-06-12T22:31:34-07:00

[original layout]
<!-- 
[User Interface](/tags/user-interface/) [Web/Tech](/tags/web/tech/) [google](/tags/google/) [web](/tags/web/) [user-interface](/tags/user-interface/) [javascript](/tags/javascript/) [web service](/tags/web-service/) [wiki](/tags/wiki/)
 -->


Life With Alacrity

© Christopher Allen