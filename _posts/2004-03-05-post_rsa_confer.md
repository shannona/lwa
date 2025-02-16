---
layout: single
title:  "Post RSA Conference Wrapup"
slug:  "Post RSA Conference Wrapup"
redirect_from:
  - /2004/03/post_rsa_confer.html
  - /2004/03/post_rsa_confer/
date:   2004-03-05 03:50:41 -0700
# image:  02.jpg
tags: 
  - Business
  - Security
  - Conference

categories:
  - news
class:
  - wide

excerpt_seperator: <!--more-->
permalink: /news/post-rsa-conference-wrapup/
---

I spent most of last week at the RSA Conference in San Francisco.

Like last year, I found little that excited me. I overheard from a convention staffer that they had 30% more attendees, so the conference is growing again, but my week there also reinforced my opinions regarding the industry as a whole as I describe in my previous blog posting [The Bad Business of Fear](/2004/02/security_crypto.html).

I asked a number of random people what they thought of the conference. Some agreed with me, saying that they were troubled by the lack of innovation. Others said that they actually liked it -- it showed that the industry was being run by businessmen finally, and not by geeks. Others said that it was just the inevitable maturation of an industry. Tim Oren wrote in his blog [Due Diligence](http://www.pacificavc.com/blog/2004/02/27.html#a565):

> Every year the show is less about cryptography per se. I'm sure this has something to do with RSA's attempts to diversify as its patents expire, but I do think it reflects the state of the field. Crypto has become a standardized component of security solutions, and the biggest perceived threats are not in the privacy area.

The hilight of the conference to me was hearing respected cryptographer Whitfield Diffie say to me that he had read my [The Bad Business of Fear](/2004/02/security_crypto.html) and that he liked it. Apparently it had been sent to him by someone at Sun who had thought that it was saying many of the things that Diffie has been saying as well. Diffie said that he had some specific criticisms, so I hope that he'll comment here someday on them.

  

#### Caller-ID for Email

The big announcement of the week was that Microsoft will be be releasing their own spam solution, a [Caller ID](http://windows-help.net/cgi-bin/2004/7.08.cgi?70801) for email addresses, starting this summer in HotMail and in their mail servers. Basically the way this works is that every domain holder publishes inside their DNS records the IP addresses of any valid outbound email server. This information is stored using XML in a special signed format. After a mail is sent, the receiving system queries the DNS to confirm that the outbound server is not being spoofed.

This is a very similar technique to what a number of other companies are proposing, for instance AOL is backing a proposal called [SPF (Sender Policy Framework)](http://spf.pobox.com/execsumm.html) or sometimes "Sender Permitted From", and Yahoo is backing [Domain Keys](http://www.eweek.com/article2/0,4149,1430976,00.asp). Unfortunately, Microsoft's Caller-ID proposal requires XML, which makes implementation much more complicated. It requires the entire email to be received by the server first, before looking up the DNS record, then validating a signature -- all of which introduces more burdens on the mail server. Lastly, this XML may exceed the 512-character limit for DNS requests, which can cause DNS servers to send via TCP rather then UDP, which may introduces even more uncertainty.

It is good to see that Microsoft, AOL and Yahoo are taking spam seriously, but I do worry that that the burden of supporting more then one of these standards may be significant. This could mean that only large corporations, educational institutions, and ISPs could host email, whereas small companies, third-world organizations, and individuals could not. I would prefer that one solution be broadly and easily adopted. <s>Daniel Goldman</s> Yakov Shafranovich in [NetWizard's blog](http://www.shaftek.org/blog/archives/000061.html) is also concerned about patent claims and lack of IETF participation:

> At the same time none of these proposals have been submitted to any standards bodies such as the [IETF](http://www.ietf.org), and as a matter of fact [Microsoft was invited](https://www1.ietf.org/mail-archive/working-groups/asrg/current/msg09082.html) to submit "Caller ID" and participate in [this week's meeting at the IETF on the subject](http://www.ietf.org/ietf/04mar/marid.txt), but [they declined](http://www.imc.org/ietf-mxcomp/mail-archive/msg00023.html). At the same time the community had jumped on Caller ID's patent license by declaring a (and [a possible incompatibility with the GPL](http://www.newsforge.com/article.pl?sid=04/02/26/1448253&mode=thread)). Of course it remains to be seen what exactly does Caller ID claim to patent since RMX and other prior art existed at least since 1998, and if Caller ID ever makes it to the IETF, Microsoft will have to deal with [the new IPR guidelines (RFC 3669)](http://www.ietf.org/rfc/rfc3669.txt) which favor non-patented technologies.

I'm also not convinced that even if these techniques are deployed (Gartner group [predicts](http://informationweek.securitypipeline.com/news/18201583) less then 25% will implement these in the next two years) that they will not return us to early 1990's levels of spam, only just slow down the onslaught. For instance, in a similar fashion to current WiFi war-chalking, a spammer could wait until an authenticated user logged in a mail server and hijack that connection. Unless the link is encrypted and authenticated, it is possible for a spammer to impersonate the legitimate user without anyone being the wiser. Related, these techniques do not necessarily help with the growing threat of "phishing" -- emails that lure unsuspecting users to enter credit card or bank account information into fake web sites.

I am also concerned that all of these standards require some measure of public-key infrastructure, including management of public-keys, which many security analysts believe that we are not doing a good enough job now.

There is some good thoughtful analysis of these three standards by Larry Seltzer of eWeek in [Who will Win the SMTP Authentication Wars](http://www.eweek.com/print_article/0,1761,a=120536,00.asp).

  

#### More Security in Windows XP SP2

Bill Gates also discussed new security features in the upcoming Windows XP SP2. In addition to some interesting "Active Protection Technology" to prevent overflow attacks, he discussed built-in virus protection and an improved built-in firewall that also warns of outbound connections.

Out in the hall I heard some people saying that announcement was a good basis for selling Symantec short, while others countered that Microsoft never gets these type of things right and there would always be business for Symantec. Companies that offer more minor features like preventing browser popups will be hurt. However, as these solutions are already free and ubiquitous, this is one of the few cases where I prefer for these to be in the default Microsoft install. However, I do worry for the smaller but more innovative security vendors like ZoneAlarm.

  

#### Sessions

Over the years the sessions at RSA have become more managerial and corporate in nature, but there were a couple of good technical sessions that I attended or friends commented on.

I was pleased by the Cryptographer's Panel response to Bill Gates' announcements: "We have a lot of great levers in cryptography, but we're missing the OSes and platforms that can really serve our keys," said Ronald Rivest. "Bill Gates didn't talk about simplifying things, but that's the only way we are going to get security. We're not smart enough to handle the complexity of this stuff. You have to get the complexity out of there," continued Paul Kocher. Whitfield Diffie criticized security the upcoming Windows Longhorn release because "For the first time, you will have a PC that does NOT do what you tell it to."

The Cryptographer's Panel also spoke on the topic of electronic voting, and supported calls for paper ballots to supplement and verify votes cast with new electronic voting technology. Rivest cautioned "We know only too well the difficulties of securing complex electronic systems."

I also heard good things about the "Hacking VM Machines" and "Analyzing Topologies of Trust" sessions, and the closing keynote by PJ O'Rouke, but I missed them -- anyone have any notes? Where there some other good sessions I missed?

  

#### Exhibits

The exhibit floor was again a bit droll for me. Like in previous years the floor was dominated by vendors selling rather high-end corporate systems that might have excited me more if I was in the market for one, but I was looking for less expensive systems for smaller businesses. Like last year there were lots of dedicated devices, such as firewalls, spam prevention, VPN and intrusion detection hardware, and fewer companies offering software to use with my existing hardware.

I did like some of the biometric hard drives, but investigating more deeply I just can't trust them yet. No one yet offers a good solution for redundant key storage yet for these, as a backup in case of a physical failure.

I did see one company [Authenex](http://www.authenex.com) that was offering free USB keys that supposedly allow you to encrypt files on your system and email them to someone else with a different key -- it looks like some public key technique is being used, with the key serving as a pre-generated private key storage. More interestingly, they claim that if you register your USB key at their website, they can send you a replacement key that you can use to decrypt your old files. I'll have to do some more investigation of the technology behind this, and if they've had adequate study by cryptographers that I trust. If they have, and they start offering storage on those keys as well, they may have something useful that I'll buy.

RSA had an demo of it's [prototype RFID blocker tag](http://www.rsasecurity.com/company/news/releases/pr.asp?doc_id=3376) that they suggest is a possible solution to some of the fears that some of us privacy advocates have been worrying about. [Scott Mace](http://scottmace.typepad.com/imanager/2004/02/cool_demo_rsa_r.html) has a good description of the demo:

> Each booth visitor selects from one of three demo prescriptions -- "tranquility pills," "wisdom pills," or "happiness pills." (I chose wisdom, naturally.) The RSA Labs crew requests a name from the visitor, then hands over an appropriately-tagged bottle (mine contained jellybeans). They scan the bottle on an RFID tabletop scanner and visitors see the details of the prescription, including type of prescription and patient's name. Then, they insert the bottle into an ordinary paper pharmacy bag that happens to contain a paper "blocker tag" that then blocks any attempt for an RFID reader to scan the bottle while it's in the bag.

Though a cool demo, I'm not as confident that this solution will work. Now in addition to the previous "foil bag" theft techniques, what prevents someone from building one of these into a watch or a PDA? Sending a signal to burn-out the RFID is one of the other proposals out there, it has similar problems -- what if someone goes into a WalMart and burns-out every RFID in the place?

RSA was also demoing its latest SecurID integration with Windows, which will extend the life of this security token for RSA customers for many years. I spoke to Scott Schnell, VP of Marketing, afterwards at a party and he explained to me some of the details of how they made it work with Windows laptops. Apparently the system will cache up to several weeks worth of SecurID information such that the laptop owner can use his SecurID token to log on to his laptop even though he is not connected to the network. I neat trick, though I'd like to see some more security reviews before I'd deploy it broadly.

Probably the most interesting, but least useful to me, was a booth for [Magiq Technology](http://www.magiqtech.com/), who offer a commercial quantum cryptography solution. Quantum cryptography is the ultimate in secret key exchange at a distance -- you can sort of say that the universe protects you from snoopers. However, you have to have a fiber-optic connection between the two devices, which limits its practicality. But it is still cool.

### Comments

NetWizard's blog is actually mine, not Daniel Goldman's (who is a good friend of mine). The patent issues important and in the ASRG which I co-chair, they have come up before with C/R patents held by MailBlocks (you can find some juice tidbits at [http://www.solidmatrix.com/research/asrg/asrg-ipr.html).](http://www.solidmatrix.com/research/asrg/asrg-ipr.html).)

[Yakov Shafranovich](http://www.shaftek.org) 2004-03-05T13:09:24-07:00

Sorry Yakov! I've corrected the attribution above.

[Christopher Allen](http://www.lifewithalacrity.com/) 2004-03-05T23:19:47-07:00

[original layout]


Life With Alacrity

© Christopher Allen
