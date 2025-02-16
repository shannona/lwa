---
layout: single
title:  "Looking at Wiki"
slug:  "Looking at Wiki"
redirect_from:
  - /2004/02/looking_at_wiki.html
  - /2004/02/looking_at_wiki/
date:   2004-02-19 16:25:05 -0700
# image:  02.jpg
tags: 
  - Wiki
  - Social
  - Social Software

categories:
  - article
class:
  - wide

excerpt_seperator: <!--more-->
permalink: /article/looking-at-wiki/
---

I've not just been spending time looking at social networking services, I've also been digging deeper into wiki. I've still got more to go, but some of these will be of interest to you if you are considering implementing a wiki for your community, or if you are a wiki developer.

[Zwiki](http://www.zwiki.org) is based on Zope, and thus has a very interesting feature set. One of the more popular features is the topic mappings that it creates. When combined with the CMS features of Plone, it becomes even more interesting -- one of the best Zwiki/Plone communities to look at as an example is [Hurricane Audio](http://doc.hydrogenaudio.org/wikis/hydrogenaudio/FrontPage). Unfortunately Zwiki only works on the Zope web platform, which is not as popular as Apache.

[FlexWiki](http://www.flexwiki.com) is a very innovative wiki that is being developed by some Microsoft engineers and is ASP.NET based for Windows. I in particular like the [property page features](http://flexwiki.com/default.aspx/FlexWiki.ExamplePropertyPage) which are an elegant way to handle meta-data, and also how it handles diffs.

[ProjectForum](http://www.projectforum.com) and [courseforum](http://www.courseforum.com) are both fairly simple but elegant commercially supported wiki. Of particular note is that both are very easy to install, even on a Windows 2000 system or Macintosh, as well as on Linux. I was able to get a test ProjectForum up on my Windows PC in about 5 minutes, including downloading. It also has some nice "skins" available. I also like how private areas are created for each -- this is the basic difference between the two products, and a rare wiki feature.

[WikidPad](http://www.jhorman.org/wikidPad/) is interesting because it is not a public service, but a shareware single-user "notepad" for Windows that supports wiki-style TextFormattingRules and WikiWords. If you have been using wiki a lot like I have, sometimes you catch yourself using wiki-style text everywhere, and I guess this product is for people who do that like me.

[SocialText](http://www.socialtext.com) is another commercially supported wiki, but is sold as a service not a product. They are very carefully added features while keeping things elegant and simple for less sophisticated business customers. They also host a number of public wikis, so if you want to see the current feature set see [RSS-Winterfest](http://http://www.socialtext.net/rss-winterfest) which also shows off their newest RSS support.

[SeedWiki](http://www.seedwiki.com) is another wiki service rather then product (sometimes called a WikiFarm), and is interesting because it doesn't use Wiki style TextFormattingRules -- instead, it has several WYSIWYG editors that allow you to directly edit the underlying HTML. This gives a huge amount of flexibility for some of the communities that use it, such as [WikiFish](http://www.seedwiki.com/page.cfm?doc=WikiFish&wikiid=1231).

I also have heard good things about PHPWiki and MoinMoin, but I haven't had a chance to dig into those very much yet.

I personally have been using [TWiki](http://www.twiki.org) for 4+ years at several of my businesses. Its strength is that it is oriented toward allowing private groups who can manage their own access privileges. It also has one of the most active 'plugins' developer areas with lots of ways to modify your TWiki to do different things (one of the plugins I'm investigating now is [GnuSkin](//http://twiki.org/cgi-bin/view/Codev/EvEm>EvEm</a>).%20My%20only%20complaints%20are%20that%20TWiki%20is%20rather%20hard%20to%20install,%20and%20that%20the%20default%20skin%20isn't%20very%20elegant%20(I%20recommend%20the%20<a%20href=), but read the docs very carefully as you have to chmod a module if you install it.)

Although it uses a fairly primitive wiki, I highly recommend the [Meatball Wiki](http://www.usemod.com/cgi-bin/mb.pl?MeatballWiki) site for people very interested in wikis. It is a meta-wiki discussion community. It has some great pages on the life-cycle of wikis, on various design patterns and features of wikis, and of various other consequences of the medium. If you look at [CategoryWikiEngine](http://www.usemod.com/cgi-bin/mb.pl?back=CategoryWikiEngine) it has one of the more complete lists of Wiki engines out there.

I will be reporting more on various wikis and wiki technology that I discover in the upcoming weeks.

### Comments

Chris, have you seen the Socialtext feature to create private areas? Other distinctive capabilities include email integration, and integrated weblogs? - Adina

[Adina Levin](http://www.socialtext.com) 2004-02-02T10:55:37-07:00

Yes, I do know about those features, but I hadn't intended for this post to be an exhaustive review, just a paragraph in or so for each. The fact that you have lots of features is why I referred people to the public rss-winterfest site. I am thinking about doing some more detailed reviews soon, though, and SocialText is near the top of the list.

[Christopher Allen](http://www.lifewithalacrity.com/) 2004-02-02T12:10:44-07:00

Check out http://tikiwiki.org/tiki-view_articles.php. Cheers Stuart

[stuart henshall](http://www.henshall.com/blog/) 2004-02-02T16:21:12-07:00

URL: Flexwiki doesn't even work with my Mozilla browser. I'd also recommend MediaWiki (used for all the Wikipedia sites), SnipSnap (java based wiki+blog), and Tiki.

[wikuser](#) 2004-02-04T10:12:49-07:00

The importance of wiki is that WikiIsDocumentBased. ( [http://communitywiki.org/WikiIsDocumentBased](http://communitywiki.org/WikiIsDocumentBased) ) IM, IRC, e-mail, all that stuff is message based. This is the first document based medium. Documents are big heavy things that float around for long periods of time. Messages are flitty things that are useful for a very short period of time. Documents are good for stabilizing massive teachings that don't change often. Messages are good for coordinations and handling new things quickly. We need both. Wiki is essential.

[LionKimbro](http://speakeasy.org/~lion/) 2004-02-09T00:14:10-07:00

PC Magazine did a review December 30, 2003 at [http://www.pcmag.com/article2/0,4149,1402872,00.asp](http://www.pcmag.com/article2/0,4149,1402872,00.asp) that rated both SocialText [http://www.socialtext.com/](http://www.socialtext.com/) and EditME [http://www.editme.com/](http://www.editme.com/) at four starts

[Sean Murphy](http://www.skmurphy.com) 2004-02-12T11:41:40-07:00

Nice post, I really enjoy oddmuse the next "version" of usemod, which I enjoy because of it's simplicity. also there are a bunch of wikis at WorldWideWiki:SwitchWiki [http://www.worldwidewiki.net/wiki/SwitchWiki](http://www.worldwidewiki.net/wiki/SwitchWiki)

[Mark](http://markdilley.2ya.com) 2004-02-14T02:26:02-07:00

URL: Voodoopad at [http://www.flyingmeat.com/](http://www.flyingmeat.com/) is a good wiki notepad for Macs, with html export. The developer is also working on an online version

[David Wilcox](#) 2004-03-03T07:16:26-07:00

The canonical list of wikis is at: [http://www.c2.com/cgi/wiki?WikiEngines](http://www.c2.com/cgi/wiki?WikiEngines) A very interesting collaborative internet medium is noosphere: http://www.c2.com/cgi/wiki?WikiEngines It is not a wiki - but it is close in the collaborative process.

[Zbigniew Lukasiak](http://zby.aster.net.pl/kwiki) 2004-03-14T06:55:59-07:00

The canonical list of wikis is at: [http://www.c2.com/cgi/wiki?WikiEngines](http://www.c2.com/cgi/wiki?WikiEngines) A very interesting collaborative internet medium [http://aux.planetmath.org/noosphere/main.html](http://aux.planetmath.org/noosphere/main.html) It is not a wiki - but it is close in the collaborative process.

[Zbigniew Lukasiak](http://zby.aster.net.pl/kwiki) 2004-03-14T06:58:16-07:00

[original layout]


Life With Alacrity

© Christopher Allen