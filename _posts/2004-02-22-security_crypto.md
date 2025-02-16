---
layout: single
title:  "Security & Cryptography:The Bad Business of Fear"
slug:  "Security & Cryptography:The Bad Business of Fear"
redirect_from:
  - /2004/02/security_crypto.html
  - /2004/02/security_crypto/
date:   2004-02-22 14:12:29 -0700
# image:  02.jpg
tags: 
  - Business
  - Social
  - Security

categories:
  - article
class:
  - wide

excerpt_seperator: <!--more-->
permalink: /article/security-and-cryptography-the-bad-business-of-fear/
---

As I head out next week to the [RSA Conference](http://2004.rsaconference.com/) I realized that it has been 13 years since I attended the first one. I remember fondly the potential and power of cryptography technology in 1991 -- public keys, digital certificates, new possibilities for privacy, digital cash, etc.

After 8 more years I left the compujter security industry on March 15, 1999. The computer security industry also seemed to be filled with as much potential as it did back in 1991. Amazon, EBay, and other Internet notables were still riding high, and driving before them the need for secure Internet transactions. The government's attempt to cripple the industry through their Clipper chip initiative was all but dead, and we were slowly winning the rights to export our technologies without severe and unnecessary government restrictions. We were beginning to truly see how Certificate Authorities worked in practical usage, and were coming up with plans for smaller, more efficient certs, to help bring security to wireless devices and set-top boxes.

It may seem strange that I left the industry at such a height, but I'd accomplished my own personal goals. I helped midwife the startup of [VeriSign](http://www.verisign.com), and digital certificates were now broadly available for both servers and clients. I'd helped fight Clipper, and freed RSAREF so that it could be used by Open Source software before the expiration of the patent. I'd grown Consensus Development, a company I founded almost a decade before, from a small engineering house into the premiere SSL developer. I'd lead the team that developed the SSL Reference version for Netscape, and had completed the IETF's [RFC 2246](http://www.ietf.org/rfc/rfc2246.txt) that described the future of SSL called TLS.

Thus I found myself at the heart of a burgeoning Internet commerce industry. When [Certicom](http://www.certicom.com), a leading cryptography company, had expressed a desire to purchase my company, I considered the returns for my investors, the value to my employees -- I was pleased with the results, and agreed. So I made an exit from the security industry, and as part of my agreement with Certicom I signed a non-compete which gave them a few years' head start before I dipped my foot back into the security industry.

Now, five years more have gone by. My non-compete with Certicom has expired and for over a year I have slowly been easing my way back into the world of security and cryptography. I must admit, I was a bit uncertain at first. Five years ago I had seen the industry perched on the edge of the next big change. It had been prepared to secure the hundreds of new applications that were proliferating on the net; to broadly adopt TLS, the newest version of SSL; to really look at the practical applications of certificate authorities and recreate the entire concept as a second generation of ideas. I wondered how far behind I would be, if I'd recognize the industry at all. Internet time had still been moving fast back in 1999 and I wasn't sure how many generations had gone by in the security industry. One, two, more?

So last year I started attending security related conferences again, such as [IETF Meetings](http://www.ietf.org/meetings/meetings.html), the [RSA Conference](http://2004.rsaconference.com/), and others. I was ready to come as a student, to soak up the new knowledge imparted in the talks and tutorials, to glory in the changes that the last five years had brought. Instead I discovered, almost nothing had changed. If anything, the industry had been moving backward, just a tiny bit.

What had happened to an industry that just five years ago had been rapidly pushing forward the frontiers of technology?

And, more important, how could it move forward?

#### The State of the Industry: Living off of Fear

Overall, I find the state of the security industry to be a bit sobering for its lack of momentum in recent years. This slowdown can be seen nowhere as easily as upon the exhibit floor of RSA Conference, the premiere conference for this industry, which I attended last year and will attend again next week.

Walking the floors of RSA last year, in the immense exhibit hall at the San Jose Convention Center, I did feel a sense of energy. The floor was still packed, and the carefully cut kiosks and the garish banners bespoke the millions put into the show by the exhibitors. The constant chatter was a deafening white noise, and whenever I veered too near a booth, there was a salesman very eager to tell me about his company's latest and greatest.

But, to a certain extent, that energy felt to me like a facade. There was nothing new; instead all the exhibitors were showing off the same technology that they were displaying five years ago. There was a bit of glitz and some extra chrome, perhaps a carefully redesigned product name, but beyond that there was a weird feeling of deja vu.

There were the same old tools that we've been using to deter hackers since the advent of the Morris Worm way back in 1989: products to detect intruders and safeguard your machines against them; firewalls; and VPNs. Maybe we've gotten a little better at figuring out expert rules, maybe we've improved our user interfaces, but these are slow, gradual upgrades, not quantum leaps.

Email still seems to be the newest battlefield upon which security wars are being fought, and you could find any number of new anti-spam tools at RSA. The Bayesian filters are a new and interesting way to statistically classify spam, but at the core level they're a dynamic outgrowth of keyboard filters that have been around for as long as we've been fighting unsolicited commercial email. RSA's big release of the year, Nightingale, was simply another way to protect sensitive online information, a competitor to Microsoft's Wallet technology. We had the ubiquitous hardware tokens too, and discussion of the recently approved AES encryption standard, but nothing dramatically new and exciting.

I suppose I shouldn't have been too surprised, based on my experiences at IETF a month before. Most of the Security Area working groups were still working on the same problems that they'd been discussing five years before. S/MIME is pushing forward on yet another draft of a standard that has never been broadly deployed. IPSEC is similarly continuing to work on the same problems, now years old. TLS was widely implemented and specified, but not widely adopted -- the world still uses SSL 3.0.

In the last year since those two conferences I had lunch with various professional colleagues that I had lost track of, continued to watch as a bystander the leading edge of security and cryptography.

As I overview the industry I have begun to feel that we'd largely abandoned the most interesting and innovative security techniques that were being discussed just five years ago. What happened to alternative public key infrastructures? What happened to attribute or role certificates? What happened to "authorization" being the next step after "authentication", or separating "security" from "privacy"?

Remarkably, if any of these topics are being considered, they seem to be moving outside of the traditional security industry. Such is the case with [SAML, the Security Assertion Markup Language](http://www.oasis-open.org/committees/tc_home.php?wg_abbrev=security), a branch of XML which seems to be doing some of the only work on attribute certificates.

With so many technologies abandoned utterly, or else given up to another computer fields, we must ask: why are we stagnating, moving backward rather than forward?

#### Fear: Outlining the Problem

I thought, could it be the result of the dot-bomb and subsequent recession? Perhaps that is part of it, but we are in denial unless we face the deeper cause. If we go on as we are the security industry will not recover with the next boom.

The decline of the security industry is based upon a basic disconnect between the business world and the security world.

Within the security industry we base our models of trust upon mathematics. We strive to continually push the envelope by codifying security and improving it. On the other hand the business industry bases its models of trust upon risk. It balances the risk of a bad outcome, the cost of that bad outcome, and the cost of reducing that risk. Even if a system is technically insecure, the business world will accept it if the risk of a security breach is low, the cost of a security breach is low, or the cost of closing that breach is high.

Where our model is mathematics, theirs is economics. These two models worked well in tandem for quite a few years; the need for a security industry was initially obvious because of the totally undefined risks and the potentially high costs that were out there, waiting to be taken advantage of.

But now, years later, we've done our job too well. We've taken all those undefined risks and codified them -- made them real and quantifiable. We've offered real demonstrations of online security through years of ecommerce, and in doing so we've proven lower rates of credit card fraud, and almost total proof from high-cost offline problems like extortion and bad reputation. We've helped fill out business' risk models and so shown when we were necessary and when weren't.

In short, we have dug ourselves into a hole. Thus it shouldn't be surprising that the newer security technologies are stagnating ... because we've carefully, cleverly, and constantly diminished our revenues by staying with a business model in which 'good enough' security will become ever cheaper. We've turned our security business into a cheaper alternative to insurance, where business only pay for security if their insurance premiums would otherwise be too high. As the bulk of the risk is now handled by old, cheap technology, what remains for new sales is not enough to keep us truly innovating.

Recent statistics underline the decreasing value of innovative, new security to businesses. According to the [CSI/FBI 2003 Computer Crime and Security Survey](http://www.gocsi.com/press/20030528.jhtml?_requestid=105732), the annual cost of computer crime has decreased in almost every category. From 2001 to 2003, the cost for theft of proprietary information is down from $151.2M to $70.2M. System penetration by outsiders is down from $19.1M to $2.8M. Insider abuse of network access is down from $35.0M to $11.8M. The only computer crime up in dollar damage inflicted is denial-of-service attacks, a very small part of the security pie.

With costs due to computer crime plunging year after year, clearly companies are not incentivized to put money in new prevention technologies.

To simplify, as long as the risks were unknown, we were in a business feeding off of 'fear' and our security industry 'pie' was growing. But as we and our customers both understand the risks better, and as we get better at mitigating those risks cheaply, this "fear" shrinks and thus the entire 'pie' of the security industry becomes smaller. Yes, new 'threats' keep on coming: denial-of-service, worms, spam, etc., but businesses understanding of past risks make them believe that these new risks can be solved and commodified in the same way.

As the philosophy and culture of the business world is hundreds of years old, going back to at least the Italian merchants of the Renaissance, business isn't going to change its model of how business works. Thus, it is up to us to rework the basic beliefs and understanding of our security industry.

In order to get out of this hole we need to dramatically rethink how we approach, develop, and market security services. To do this requires us to reconsider our own security models, based upon a better understanding of core business models. Some possibilities:

1.  [Enter the Insurance Business](#insurance)
2.  [Move into Reliability Improvement](#reliabiliy)
3.  [Move into Enabling Technologies](#enabling)

#### Solution #1: Entering the Insurance Business

Entering the insurance business is an old idea. It was once an important part of [Verisign's](http://www.verisign.com) business plan, and no doubt of others as well.

At its simplest level, we can enter the insurance business by offering a guarantee against damages with a product. The main benefit of this approach is that it lets us approach security in a more rational and realistic fashion. No longer do we have to engage in an endless quest for improved security, no matter how small the risk. Instead we can assess our risks and prepare ourselves to accept manageable losses.

There are risks implicit in this solution as well. For the most part, those of us in the security industry are unfamiliar with the insurance business model, and thus we're entering particularly uncharted waters. In addition, we need to understand that some losses will be huge and unavoidable, such as was the case with the Code Red worm. We thus need to create business models that are acceptable to our customers, but which do not leave us entirely liable for the next utterly unforeseen worm which gets set loose on the Internet.

There may also be some limitations with this particular model, if the valuations of security companies are too low to insure the losses of a large corporation, such as a GM.

Finally, we need to ask ourselves the question: "What value does insured security provide over simple insurance?" I suspect there are some real values to customers in saved productivity and time, but further market research would be required to truly assess this.

A security company could offset most of these risks by a partnership with an insurance company or another business within the insurance industry. We would need deep reserves and to work together with imaginative actuaries. Together we could offer insurance against the damages of security breaches. We would be the guardians against break-ins and the fixers if they did occur. The insurance company would help estimate risks, collect premiums and pay.

If we chose to go it alone, we could offer risk mitigation services to insurance companies. We would guard and provide disaster mitigation services for a monthly premium. For example, when offering an anti-breakin security system, we could offer a guarantee to rebuild all certified systems if an intrusion does occur. This way we would take some, but not all, of the risks. Perhaps our presence would reduce insurance premiums enough to pay for our fees.

Overall, despite potential risks, I believe that using an insurance model is a strong possibility for the security industry.

#### Solution #2: Improving Reliability

Some of us in the security business may feel like we are already providing reliability, because many of our products prevent catastrophic risks due to break-in, theft, and other malevolent acts. However, what we generally tend to offer is data security, not data reliability. Perhaps paradoxically, at the more personal, day-to-day level, the security industry has actually reduced data reliability in the name of improved data security.

I can personally testify to this fact because I have, recently, lost data due to security. I encrypted a directory in Windows XP, then was later forced to rebuild my system. Apparently some of the required info to decrypt the directory was stored in some unrecoverable registry entry, because I can no longer access it. The data is totally secure, but also unavailable.

This anecdote isn't unusual for the security industry. Forgotten keys can often cause cryptographic-related data loss. Likewise, VPNs and firewalls introduce single points of failure into networks.

RSA's Nightingale technology of last year is a fairly standard security-based technology. It uses "secret-splitting" technology to divide sensitive data among two different locations, thus removing what RSA calls "a single point of compromise"; you can't get access to the data unless you compromise two machines. Clearly, there is improved data security. However it raises the same old problem of data reliability, because now data can be lost if either of two servers is lost.

Improving reliability of extant security protocols is a good move forward in this expansion of the industry. For example in a classic cryptography situation we might unlock data with multiple secrets, but only require a set number of those secrets to unlock the data, not all of them.

Consider a company who is encrypting some of their most sensitive sales and marketing data. Ten company officers might each possess a secret which together can be used to decrypt all the data. However, this introduces a clear reliability problem, as the departure of any officer could leave all sales and marketing data unreadable. (Likewise, just restricting this data access to one specific secret, such as that of the VP of Sales, introduces this single-point-of-failure condition.) Instead we could offer a high reliability, but secure situation where any five (of ten) secrets together could decrypt the data. Therefore, if an individual officer disappears, leaves for a rival company, or otherwise makes his secret unavailable, not only can he himself not access the data alone, but even if he leaves with the secret the remainder of the company's access is unaffected. And, if a company didn't think that "5 of 10" executive was the right number, they could instead only require "3 of 10" to decrypt the data ... or "7" or "9".

By thinking in this new methodology, by measuring security against reliability, we can offer our customers real choices and let them each choose the level of security that works best for them.

However, the underlying bases of cryptography let us go a step further than this. Even without considering security implications, we can make use of our existing cryptographic algorithms in order to allow for more reliable access to and retrieval of all sorts of data. In other words, we can offer protection against not just hackers, but also backup errors, system crashes, and other catastrophic failures that are actually much more likely to affect the average user than an Internet security breach is.

[iSCSI](http://www.ietf.org/html.charters/ips-charter.html), a remote SCSI protocol, offers very good potential for interaction with cryptography. A redundancy caching technique, somewhat like RAID 5, could be integrated with a secret share system where, e.g., the data could be read as long as 80% of the remote drives (and thus their keys) could be accessed; this allows for a very high reliability storage system because individual storage drives could be distantly located, and at the same time uses cryptographic techniques to offset reliability problems that could potentially be caused by the uncertain and fluid nature of Internet connectivity.

Even issues like load balancing and methods to deal with machine down-time might all be improved by some of our cryptographic techniques.

#### Solution #3: Leaving Behind Fear

In talking about insurance and reliability I feel like I'm largely expanding upon a fairly well-known and conservative way of using cryptography. These are good first steps for companies that wish to move forward in a cryptography market that is shrinking due to our own success, but they're not necessarily enough for a major breakout into revenue sources that will make this once again an exciting industry from a business point of view.

What is required, I believe, is a major paradigm shift. We need to leave the whole business of fear behind and instead embrace a new model: using cryptography to enable business rather than to prevent harm. We need to add value by making it possible to do profitable business in ways that are impossible today. There are, fortunately, many cryptographic opportunities, if we only consider them.

Cryptography can be used to make business processes faster and more efficient. With tools derived from cryptography, executives can delegate more efficiently and introduce better checks and balances. They can implement improved decision systems. Entrepreneurs can create improved auction systems. Nick Szabo is one of the few developers who has really investigated this area, through his work on [Smart Contracts](http://www.firstmonday.dk/issues/issue2_9/szabo/). He has suggested ways to create digital bearer certificates, and has contemplated some interesting secure auctioning techniques and even digital liens. Expanding upon his possibilities we can view the ultimate Smart Contract as a sort of Smart Property. Why not form a corporation on the fly with digital stock certificates, allow it to engage in its creative work, then pay out its investors and workers and dissolve? With new security paradigms, this is all possible.

Federated identity is another area for potential expansion. Secure, federated identities could offer many benefits for consumers. Imagine being able to visit a third-party seller on the Internet, automatically charge a sale to your Amazon account, then automatically ship it to your standard address, all through a single secured identity token. Federated network identity also has real applicability in the business world, as is shown by the work being done by [Liberty Alliance](http://www.projectliberty.org/). Through a business system like this, an auto parts manufacturer could offer his products to General Motors as part of a larger bid, all without having to specifically arrange identity with GM itself.

However, there are notable challenges in the area of federated identity -- challenges which a new-paradigm security industry could lead the way in solving. Distinctions must be made regarding various levels of identity security, so that, e.g., your VPN couldn't be accessed if someone gained access to your Amazon password. In addition there are real concerns from users about controlling their user information, due to worries over spam and privacy; some users, for examples, might not want information about their politics, sexuality, or interests federated with information about their family or job. For instance do we really want our information on [Orkut](http://www.orkut.com) to be used by [Google](http://www.google.com)?. These challenges demonstrate why federated identity is still a leading edge possibility for the security industry.

Beyond business processes and federated identity there are many other areas that the security industry should be considering, as it moves beyond the business of fear. The whole idea of Public Key Infrastructures should perhaps be rethought, and maybe we should resuscitate lost technologies such as Attribute Certificates, and some of the ideas such as local name spaces as in described Rivest's [SDSI](http://theory.lcs.mit.edu/~cis/sdsi.html). There are also some interesting possibilities for trusted peer-to-peer environments that can be dynamically expanded on the fly. The possibilities are only limited by our imagination, if we can just think beyond current possibilities.

We have already seen the first wave of security technology; now we need to initiate a second, for I believe with the next wave the best is yet to come.

### Comments

Just thought I would comment that in building actuarial tables, insurance companies have a relatively small set of policy-holder behaviors and traits. Auto insurance underwriters look at age, vehicle model and model year, zip code, driving history, and maybe a few more traits. How do you even start to build a table for the computer industry? You're running Windows? Fine, double your premiums. You're running Windows 95? Great, double them again. You haven't updated your router firmware in three months? Well... what does that do the measure of risk? Anything? I've always really liked the idea of IT insurance as a way to drive effective, practical security protections, but I think we're light-years away from collecting enough information to build a reliable actuarial table.

[Matthew S. Hamrick](http://www.cryptonomicon.net/) 2004-03-03T14:30:44-07:00

I enjoyed this article. The RSA expo floor really makes me feel sad nowadays. It has really driven home the lesson that security is not, as I once believed, a tool that naturally lends itself to increasing freedom. Instead, like all tools, it cuts either way depending on the hand that guides it. I remain hopeful that capability access control will be deployed and will enable, in Mark Miller's phrase, "cooperation without vulnerability". The concept of mutually untrusting code (operating on behalf of mutually untrusting people) cooperating in a single address space is a paradigm that the MUD culture has been practicing for at least a decade and that the Java culture is likely to discover in 2004. The increasing importance of virtualization, Trusted/Treacherous Computing, and the like also lead us closer to this paradigm.

[Zooko O'Whielacronx](http://zooko.com/log.html) 2004-03-04T05:48:07-07:00

URL: So then one day this guy discovers the answer to the Reimann Conjecture and now Fear and risk are en vogue again. I was curious what you think might be the replacement for prime number pki?

[Joe](#) 2004-09-07T06:23:57-07:00

[original layout]

Life With Alacrity

© Christopher Allen