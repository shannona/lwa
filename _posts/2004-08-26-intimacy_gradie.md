---
layout: single
title: "Intimacy Gradient and Other Lessons from Architecture"
slug: "Intimacy Gradient and Other Lessons from Architecture"
redirect_from:
  - /2004/08/intimacy_gradie.html
  - /2004/08/intimacy_gradie/
date:   2004-08-26 16:56:26 -0700
# image:  02.jpg
tags: 
  - Security
  - Social Software
  - Wiki
  - Web/Tech

categories:
  - article
class:
  - wide

excerpt_seperator: <!--more-->
permalink: /article/intimacy-gradient-and-other-lessons-from-architecture/
---

A number of my posts have been about integrating different domains of knowledge in order to better understand how human behavior should be incorporated in the design of social software. I found [The Dunbar Number](/2004/03/the_dunbar_numb.html) in sociology, and both [Four Kinds of Privacy](/2004/04/four_kinds_of_p.html) and [Progressive Trust](/2004/08/progressive_tru.html) come from my work in the cryptography field. The topic of this post comes from the field of architecture.

In order to provide for [Progressive Trust](/2004/08/progressive_tru.html), you need to establish what is known as an "Intimacy Gradient".

The concept of Intimacy Gradient comes from architect Christopher Alexander, in his book [A Pattern Language: Towns, Buildings, Construction. (Oxford University Press, 1977)](http://downlode.org/etext/patterns/):

> _[Pattern #127 - Intimacy Gradient:](http://downlode.org/etext/patterns/ptn127.html)_
> 
> _**Conflict:** Unless the spaces in a building are arranged in a sequence which corresponds to their degrees of privateness, the visits made by strangers, friends, guests, clients, family, will always be a little awkward._
> 
> _**Resolution:** Lay out the spaces of a building so that they create a sequence which begins with the entrance and the most public parts of the building, then leads into the slightly more private areas, and finally to the most private domains._

In architecture there are always some areas of the house or building that are more public -- the entry, the living room, the atrium, etc., and areas that are more private such as bathrooms, bedrooms, and offices. In a good design there is some marker of change between these different areas -- it might be a difference in ceiling height, a stairway leading to a different floor, or a narrow entrance. As an example, in the classical Japanese tea house, you have to bow low before entering.

Failure to respect the Intimacy Gradient results in uncomfortable buildings. [Tom Munnecke](http://munnecke.com/gehry.htm) reported about a Frank Gehry building at Case Western Reserve University:

> _I asked many of the graduate students how they felt about their new environment. "Horrible," said one. "Like living in a refrigerator" said another. "We used to have comfortable offices and gathering places, and had the most wonderful conversations. Now everything is so sterile, and the acoustics so bad, that we can't do anything together. I have to go outside if I want any privacy."_

The Intimacy Gradient is also used in other media. As I noted in my review of [Seven Fingers of the Hand Circus](/2004/01/seven_fingers_o.html):

> _When we arrived, we were led down the side of the theatre and all of a sudden I noticed that it looked like we were all being led backstage. We curve around and all of a sudden see an entrance -- maybe 5 foot tall requiring most of us to duck. We duck through and to our surprise, we are have walked through a fridgerator, and we are on the stage!_
> 
> _One of the 7 players welcomes us, and another offers random people a glass of tea as we walk across the stage to our seats. The stage is set like a city loft, with a tv, some couches, a bed, a bathtub and shower, a kitchen, and of course the fridgerator we entered through. On the stage, and chatting to members of the audience are the 7 cast members, all wearing comfortable looking white shorts or athletic and white t-shirts._
> 
> _The audience arrives over 30 minutes and the 7 players act as if we are guests of their loft, serving some of us tea, chatting, sweeping the floor, etc._

Entering through the refrigerator door raised the intimacy of the experience for the audience of that circus. Thus in spite of it being produced in a large auditorium it felt as up-close and personal as did the much smaller [Circus Contraption](/2004/08/circus_contrapt.html).

The Intimacy Gradient exists in movies as well -- anywhere you see a scene taking place in a public space that transitions down through smaller and tighter shots ultimately to a closeup of a face it is much more intimate then just cutting to the closeup.

In social software design, there also needs to be an Intimacy Gradient. One of the problems with Wikis is that there is often very little transition between public and intimate, and doing so can be quite jarring. SocialText, a Wiki service vendor, is aware of this problem and is ["seeking to add more layers to the 'intimacy gradient', without recreating the highly structured collaboration tools that exist today"](http://alevin.com/weblog/archives/001393.html). Ross Mayfield outlines [this possible future Intimacy Gradient for SocialText](http://www.corante.com/many/archives/2004/08/12/collaboration_cases_and_spaces.php):

> * _The broadest tier is a guest space, available to all_
> _* The second tier is a knowledgebase, accessible to all employees and contractors
> * The third tier is product development, for employees and contractors bound by a confidentiality agreement
> * The fourth tier is for the core management team to share confidential financial and HR information._

These thoughts from an earlier post by Ross are also thoughtful:

> _He is right that groupthink is avoided by a social network structure that allows a dynamic and diverse periphery to provide new ideas, but the core of the network needs to be tightly bound to be able to take action._
> 
> _That's the main point of Building Sustainable Communities through Network Building by [Valdis Krebs](http://www.orgnet.com) and June Holley. When studying a [community over time](http://radio.weblogs.com/0114726/categories/socialNetworks/2003/01/07.html), they suggest a vibrant community is made up of four stages:_
> 
> _
> 
> 1.  Scattered Clusters
> 2.  Single Hub-and-Spoke
> 3.  Multi-Hub Small-World Network
> 4.  Core/Periphery
> 
> _
> 
> _The ideal core/periphery structure affords a densely linked core and a dynamic periphery. One pattern for social software that supports this is an [intimacy gradient](http://www.jacana.org.uk/pattern/P127.htm) (privacy/openness), to allow the core some privacy for backchannelling. But this requires ridiculously easy group forming, as the more hardened the space the more hard-nosed its occupants become._

This is not just a problem for Wiki. There is an excellent paper on the web called [Design Patterns for Private and Public Digital Spaces in the Home Environment](http://www.ai.mit.edu/~konrad/docs/IJMMS-patterns-junestrand-keijer-tollmar.pdf) where they explore how people used VNC (video-mediated communications, or more colloquially video-chat). They state:

> _The earlier "public" character of a traditional farmer's house or bourgeois flat (in Sweden) has disappeared with the modern housing planning. Instead, distinguishing the public from the private has become central during the industrial age, with the dwelling as an exclusively private place. Now, with the transition to an information society, it seems as if the concept of public space in the private dwelling has to be reconsidered, which also means that the borders between the private and the public at home have to be opened up._

The need to provide for an Intimacy Gradient in social software is clear; however, the techniques for showing the transitions between the gradients are not. For instance, in the original Netscape Communicator, when you connected with a secure SSL connection, the border around the edge of the window would turn blue, and a solid blue key would show up. However, most people didn't notice this change and no current browser does this; even the little locked icon at the bottom of Internet Explorer and often isn't visible if you have the status bar turned off or if you are using frames.

[Flemming Funch](http://ming.tv/flemming2.php/__show_article/_a000010-001289.htm) (and [mirror](http://www.redtailcanyon.com/items/278391.aspx)) notes part of the difficulty is:

> _As long as a certain chat room or Wiki page is accessible directly with a deep link, it is going to be very hard to make it feel more intimate than any other place I can reach with similar ease. So a hierarchical structure of links doesn't do it. On the web you can't force people to accept your hierarchy if it is all just links._

Part of the solution might come from the architecture world as well -- here are some other Patterns by Christopher Alexander (see the link for Alexander's resolutions for each):

* [Pattern #31 - Promenade:](http://downlode.org/etext/patterns/ptn31.html) Each subculture needs a center for its public life: a place where you can go to see people, and to be seen.
    

* [Pattern #61 - Small Public Squares:](http://downlode.org/etext/patterns/ptn61.html) A town needs public squares; they are the largest, most public rooms, that a town has. but when they are too large, they look and feel deserted.
    

* [Pattern #69 - Public Outdoor Room:](http://downlode.org/etext/patterns/ptn69.html) There are very few spots along the streets of modern towns and neighborhoods where people can hang out, comfortably, for hours at a time.
    

* [Pattern #42 - Sequence of Sitting Spaces:](http://downlode.org/etext/patterns/ptn142.html) Every corner of a building is a potential sitting space. But each sitting space has different needs for comfort and enclosure according to its position in the intimacy gradient.
    

* [Pattern #147 - Communal Eating":](http://downlode.org/etext/patterns/ptn147.html) Without communal eating, no human group can hold together.
    

Other lessons for social software from the architecture world are the concepts of "refuge and prospect", the "savanna theory", and "defensible space".

_Refuge and prospect_ come from the landscape architect [Jay Appleton](http://www.landscaperesearch.org.uk/extra31/refuge.htm). Prospect is a place where we can see others, and refuge is a place were we can retreat and conceal ourselves. A specific prediction of his theory is that people prefer the edges of a space more then the middle. Often prospect and refuge are in conflict, as a prospect tends to be expansive and bright whereas a refuge is small and dark, but there are cases where they are combined in one place; this is why we value private homes with a spectacular view so much, and why we pay so much to stay at [scenic retreats](http://www.djc.com/news/ae/11127729.html). So what are the edges of our social spaces? Are there ways that we can signal either prospect and refuge?

The _savanna theory_ comes from a hypothesis by [Richard Coss and Gordon Orians](http://notes.utk.edu/bio/greenberg.nsf/0/f60081ef35fba95c85256e6e006a2a77?OpenDocument) that we should be most comfortable with those landscapes where humans spent most of their evolutionary past. Thus supposedly the ideal landscape design has the same proportionality of trees, grass, and brush as the African savanna; parks and golf clubs are shown as evidence of this theory. An alternate to this theory is that we desire a certain amount of [visual complexity](http://evolution.anthro.univie.ac.at/institutes/urbanethology/student/html/erich/synekpro.html). Either theory raises this question: what are the evolutionary markers regarding groups that our human ancestors needed? This question fits well with my thoughts regarding the [Dunbar Number](/2004/03/the_dunbar_numb.html).

The _defensible space_ concept comes from the idea that anonymous spaces lead to problems because of vandalism, incivility, and crime, and to eliminate those problems requires the residents to mark their "territories" and "take possession" of their areas. We have similar problems in the online world. So maybe the answer is similar -- allow more ways for groups of people to mark up and take possession of their own virtual spaces.

There are a couple of links that integrate these ideas in architecture that you might find useful:  

* [Psychosocial Value of Space](http://www.wbdg.org/design/resource.php?cn=0&rp=181)
  
* [Building Biophilia: Connecting People to Nature in Building Design](http://www.edcmag.com/CDA/ArticleInformation/features/BNP__Features__Item/0,4120,22486,00.html)
  
* [Bio-Inspired Design: What Can We Learn from Nature?](http://ceae.colorado.edu/~amadei/CVEN4838/BioInspire.1_%2001.15.03.htm)
  
* [Evolutionary Architecture: A Field Course](http://evolution.anthro.univie.ac.at/institutes/urbanethology/archi/archi.html)
  
* [Why We Say It With Flowers](http://www.the-scientist.com/yr2001/nov/opin_011126.html)
  
* [Evolutionary Psychology and Workplace Design (pdf)](http://www.contemporary.ab.ca/ke/content/pdf/evolutionary_psychology.pdf)

We are still breaking ground and exploring new ideas in the world of social software. However, there are already extant fields of study which may give us insight into this new venue. Architecture is one of them. By better understanding ideas of intimacy gradients, pattern language, refuge and prospect, savannas, and defensible spaces, we may gain new understandings of how to build social environments which are attractive and enjoyable to more people.

### Comments

Tried to post this elsewhere and failed. Sorry if it's duplication. If a person loading a page has an identity or role (one could have many of these for different purposes) then the system serving the page could show different sets of links based on the "privacy level". Of course, one could show entirely different sets of links to different people. This du(multi?)plicity would also reflect the method commonly employed in social manipulation, i.e. saying different things to different people based on one's view of them. As it stands, this suggests that the person providing the link sets owns the server, which is often not the case. Alternatively, it suggests that one is happy to trust a service provider with one's most intimate secrets. I suspect neither needs to be the case if cryptography is used.

[me](http://example.com) 2004-09-20T02:05:57-07:00

URL: The fridge door speaks to another one of the Pattern Language patterns -- that a doorway should truly be a noticable, transforming experience. That is, a clear indicator that you have gone from "there" to "here." Off-topic, I know. But interesting.

[Charlie](#) 2004-10-08T13:04:26-07:00

Thanks for the great summary and roundup of key concepts, theories and techniques from architecture and urban planning that can be applied to social software design. I'm also a big fan of these fields and I think we can stand to have a lot more cross-pollination between the worlds of software, and of space/place design. As for how to simulate intimacy gradients, and more basic, "hardwired" ways that we behave in spaces and places, in the online world (or how to symbolize or substitute for them), I wonder: Why don't we cheat more often? People use our software in spaces and places, after all. Instead of trying to -simulate- the physical, real-world intimacy mechanisms that we've evolved to use, why not just -use- those physical mechanisms and context cues that already exist? Why not design software that's aware of the very different places we move through? Why not design software and devices tied to places? That's what we're trying to do in a few very specific ways with PlaceSite.com, but there's so much more that can be done here. Sean

[Sean Savage](http://www.cheesebikini.com) 2006-07-05T22:04:01-07:00

[original layout]

<!-- [Security](/tags/security/) [Social Software](/tags/social-software/) [Web/Tech](/tags/web/tech/) [Wiki](/tags/wiki/) [intimacy gradient](/tags/intimacy-gradient/) [social software](/tags/social-software/) [collaboration](/tags/collaboration/) [wiki](/tags/wiki/) [socialtext](/tags/socialtext/) [interface design](/tags/interface-design/) [sociology](/tags/sociology/) [architecture](/tags/architecture/) [design](/tags/design/) -->

Life With Alacrity

© Christopher Allen