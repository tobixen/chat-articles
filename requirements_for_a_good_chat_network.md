This article is published on Steem: https://steemit.com/technology/@tobixen/requirement-for-a-perfect-chat-service-freedom

-----

I touched base on the history of chat networks and problem of siloization in my previous post [The great chat fragmentation](https://steemit.com/technology/@tobixen/the-great-chat-fragmentation).  I will go on and describe what I want from a perfect chat network: it should be free, it should be secure and it should be feature-rich.  This post will elaborate on the first of those three points - freedom.

![Drawn by author, released as Public Domain](http://github.com/tobixen/chat-articles/raw/master/liberatechat.png)

# Summary first

Under the "freedom" umbrella, I have those points:

* No significant cost to use
* No lock-in
* Accessibility and universal usability
* FOSS
* Open standards

Some of them may be a bit at odds with each other and at odds with security and functionality.  For instance, the possibility of future profits can really speed up investment, development and marketing - and marketing may be needed to get a critical mass of adoption - but it's very hard to combine profit with freedom (though, Steemit seems to have managed to crack that nut).  "Open standards" also tends to become stuck - nobody can design the perfect standard from scratch, and a standard cannot easily be changed if it implies a whole ecosystem of applications needs to be upgraded.  I'll discuss more on this later.

# Free as in gratis - no cost

One is often regarded as a miser if one is reluctant to pay and demanding that some service should be free.  The old phone network and SMS'es are paid services.  There are certainly benefits with this - one should perhaps expect higher reliability and availability from a paid-for service than for some free service, it's to some extent working as a deterent against spamming (but maybe not so much - I do get a decent amount of spam both to my physical paper-mailbox as well as to my telephone), it may cause better utilization of resources ... and it does require resources to build and maintain a perfect chat service - someone has to pay, directly or indirectly.  There ain't no such thing as a free lunch.  Actually I wouldn't mind paying a bit for a decent chat service, except, if it wasn't for ...

* It pretty much has to be gratis to be able to compete in todays market.  Prices for voice calls and SMSes are on the way down, and flat-rate billing plans with unlimited voice and SMSes aren't unheard of today.
* In a complicated network (i.e. the telephone network!) distribution of income among the different providers involved in setting up a connection may be a hard nut to crack - billing and cost counting may be a big cost driver by itself.  An ideal chat-service is decentralized, based on open source and with lots of contributors - in such an environment it can be difficult to collect, process and distribute an income.
* Metered usage payments for a service where the actual cost of usage is insignificant may be bad, as it causes "customers" to spend energy figuring out stupid ways to save money (anecdotes from the real world: telephone-based protocols where information is encoded in the number of rings before the caller hangs up, SMSes without spaces but using capital letters for marking the word boundaries, some russian telecom provider did allow people to call internationally for ten seconds without billing - causing some customers to make hundreds of calls muttering some few words on every call).  Actually, for chat services it can often arguably be a good thing that the sender thinks three times before sending the message - the sender is quite often significally underestimating the time costs of writing the message, as well as context-switching and reading the message on the other side.
* It's also important to consider the income inequities - in some parts of the world a cup of coffee from a café can cost as much as 10 mBTC, and most people finds it affordable - in other parts of the world, 90% of the population makes less than 10 mBTC pr day, and it would be madness to waste a days salary on one cup of coffee!  A price per message that seems really insignificant for some of us may be deemed so expensive that others are excluded from the network.

Would you use a paid-for chat service?  Feel free to tell in the comments :-)

![Andrew Butko [GFDL 1.3 (www.gnu.org/licenses/fdl-1.3.html) or CC BY-SA 3.0 (http://creativecommons.org/licenses/by-sa/3.0)], via Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/0/01/%D0%A2%D0%B5%D0%BB%D0%B5%D1%84%D0%BE%D0%BD_2.jpg)

# No evil plans for future profit generation

A service may be "gratis" without really being free - and those services may actually be the worst, I think it's better with honest, up-front payments than service providers giving away services for free and having some secret, potentially evil plans on how to turn it into a future profit.  It's not unusual that a service requires people to read through and accept a very long end user agreement - almost nobody actually takes the time to read through all of it, and often the text contains things that no sane person actually would agree on.

It's not unusual that service providers collect all kind of personal information, even scouring through the conversation content and sell it to third parties, eventually bombard the user with targeted commercial ads.  Being bombarded by targetted commercial ads may by some be seen as a good thing, targetted spam is at least more relevant than random spam - but remember, for someone to send targetted spam on a chat network, they would need to analyze all sorts of private information.  If you just shrug and think that's ok, then I recommend reading the [scroogled](http://blogoscoped.com/archive/2007-09-17-n72.html) short story.  Another anecdote, there was a story about a banking/insurance company buying up a popular supermarked chain (Tesco in the UK if I remember correct), and someone did a bit of research into what kind of insurance offers one would get with and without a Tesco frequent shopper bonus card.  Apparently the shopping history mattered a lot; people with a "healthy family shopping pattern" got quite good discounts compared to customers without a shopping card, people who frequently bought beer and cigarettes got a worse quote.  Consider that some kinds of insurance may be mandated by law (i.e. auto liability insurance) ... next thing, insurance companies doing data mining on your private chat history before giving you an offer.  Is that OK?  I think not ...

Even untargetted marketing ads may be considered evil.  It's annoying, and among other things it may consume expensive bandwidth, precious battery power and the purpose of the marketing is to get YOU to spend money on things you probably shouldn't be spending money on.  A service cannot be considered "free" it it's not free from marketing ads - though arguably financing stuff through marketing ads may be more fair towards the have-nots than financing stuff through usage fees.

How do you feel about services financed through promoted contents on the internet?  Feel free to tell in the comments :-)

![By Thierry Gregorius (Cartoon: Big Data) [CC BY 2.0 (http://creativecommons.org/licenses/by/2.0)], via Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/b/b3/Big_data_cartoon_t_gregorius.jpg)

# [Accessibility](https://en.wikipedia.org/wiki/Accessibility) - possible to use for anyone, on any platform

This is quite important, I'd say - a service that can be used by 99% of the population is simply not good enough.  People are often biased, not seeing the inherent restrictions there may be on a product, here are some examples:

* **Impairment compatibility**: A perfect chat system should be possible to use also for people with different kinds of impairment.  Yes, doing a text chat with the visually impaired is fully possible - there are specialized software for translating the screen content to spoken text, but if the only available chat client is some complicated GUI client and no text user interface client exists it may be difficult to operate.  Doing a voice chat with someone that can't hear is slightly more difficult.  At least here in Norway there was (is?) a government-paid service with human translators working as a gateway between the old telephone network and specialized text chat terminals for the hearing impaired.  Today I think it's better to just use text chat from end to end.

* **Phone number as identifier**: Maybe some 98% of the adult population has a personal telephone number and a mobile phone, but a perfect chat service should cater for 100% (even including children), not only 98%.  Some chat platforms are using telephone numbers as identifiers and text messages as authentication method.  It's all fine and dandy for most of us - but then again, there are people who denies using cellphones for various reasons, so this is no good.  A service using telephone number as identifier should at least provide some workarounds.

* **Cross-platform support**: Other chat platforms may provide an android app and an iPhone app - and maybe even an app for the windows phone.  Everyone has one of those three anyway, right?  Wrong!  And even if it was true ... among those that are using those platforms, there are people who couldn't afford upgrading the phone for some years - stuck with old hardware and probably also an old version of the operating system, and probably the latest version of the app won't work anymore.  People like me (SailfishOS - but it does support android apps) may also have a strong desire to be able to do chatting from the laptop or desktop computer.  (Generally, things have improved quite a lot over the last decade - but earlier I would quite often find myself excluded because I run Linux instead of Windows, and generally don't use any Microsoft products at all).
* A bit similar, a chat platform based exclusively on a desktop application or an advanced web application may not work at all on mobile devices.  A person sitting by the computer screen all day may not think about this restriction.  (Generally things have improved during the last decade, earlier quite many web pages was optimized for screens with resolution 800x600 - anything smaller and the web page would be hard to navigate and read, anything bigger and it would look very ugly).

* **Ease of use**: It needs to be accessible also for "ordinary" people.  Quite some technologies have failed gaining adoption because it has failed appealing to ordinary folks.  We need a chat system that can be *easily* used by the majority of the population.  Even though I just said using telephone numbers as identifier is a bad thing and that relying on android/iphone apps is a bad thing, but it may still be important to have android and iphone apps that can tap into the internal phone book (or CardDAV backend) and map your friends with people that are available in the chat network.  The important thing is just that it should still be possible to connect to the network for people who don't have a telephone number and don't want to share information about their personal network with neither the app nor the network servers.

Is this nonsense?  You probably only need to chat with the 98% normal people out there, and use other means of communication towards the freaks who don't want to be part of the network?  Feel free to tell in the comments :-)

!["Stolen" picture - haven't managed to find the origin](http://www.bluebadgestyle.com/wp-content/uploads/2013/07/disabled-toilet-down-stairs.jpg)

# Free and open source software

I'm almost exclusively using [open source and free software](https://en.wikipedia.org/wiki/Free_and_open-source_software).  What's in it for me?  Quality and freedom.

Quality: It used to be a common perception that proprietary closed-source software products had the best quality, backed by well-funded companies with professional programmers and good software development processes - while the free products was flimsy hobbyist projects.  This may have been the truth in the 80s and early 90s, but nowadays it's often quite the opposite, open source products tend to excel on everything except marketing.  It's not so that one automatically gets quality by chosing open-source products - one has to do some due diligence and chose products wisely - but at least one has the chance to do due diligence!  I usually spend some few minutes "peeking under the bonnet" to see if the code looks sane or not. In most open-source projects one can follow the development process carefully - it's like having a look into the kitchen of the restaurant before deciding if it's a good place to eat.

Freedom: It rarely happens that I'm getting my hands dirty and actually do modify open source software products - but it happens.  If something doesn't work as intended for me, or if I want to use the product for other purposes than what the original creator intended, then I'm free to fix things.  If I can't do it due to constraints on my time or skills, then I can pay someone to do it for me.  It's quite trivial to offer a bitcoin bounty for whomever fixes a feature, I can ask anyone on the market ... while with unfree software I'm totally dependent on the company that developed the software.  If the company goes bankrupt or decides to can the product ... though luck.

I could write a lot about why I have a very strong preferance for free software, maybe there will be another post some day.  Do you think it's unimportant?  Feel free to tell in the comments :-)  

![By Gregor Richards, inspiration by Harrison Metzger [CC BY 3.0 (http://creativecommons.org/licenses/by/3.0)], via Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Free_Software_and_Open_Source_Software_Composite_Logo.svg/500px-Free_Software_and_Open_Source_Software_Composite_Logo.svg.png)

# Open standards

It is important that one is free to create other products to connect to the network - it may be competing client, complimentary software, software made for some particular device, for the impaired etc.  One may want to create gateways for connecting different chat-networks or services sending relevant notifications to a group or an individual, etc.  To allow this, it's important that the standard (aka protocol) is well-defined, and it's important that there are good frameworks for improving the standard and resolving conflicts.

Unfortunately, the latter may be in conflict with the first.  Once one has an established standard and a big ecosystem of independent software using the same standard, it may become difficult or even impossible to fix flaws in the standard or develop it further. [IRC](https://en.wikipedia.org/wiki/Internet_Relay_Chat) has many flaws and lost its network effect because some of its administrators couldn't agree on how to develop the standard (as I've touched upon in [The great chat fragmentation](https://steemit.com/technology/@tobixen/the-great-chat-fragmentation).  Usage and reliability of email has stagnated because it's too difficult to evolve the standard, particularly, no good and universally agreed-on mechanisms for fighting spam has been established.  [Bitcoin](https://en.wikipedia.org/wiki/Bitcoin) may also be in serious trouble - I've touched on how bad the environment has become on Reddit in [The big Reddit Bitcoin schism](https://steemit.com/bitcoin/@tobixen/the-big-reddit-bitcoin-schism), but the issue at hand is disagreement on what direction the protocol should be evolved in.  The latter is a bit ironic as Bitcoin as of 2017 isn't a defined standard - there is one widely used reference implementation that defines the standard.  The biggest problem is that all actors in the network must be given sufficient time to upgrade should there be made backwards-incompatible changes to the standard.

With a well-thought-through flexible standard it's possible to extend the standard without breaking backward compatibility; new features will be visible for clients supporting the new feature, while old clients may degrade gracefully. [XMPP](https://en.wikipedia.org/wiki/XMPP) is designed to be extensible.  Bitcoin has also evolved from 2009 to 2017 without breaking backward compatibility; part of the conflict in the Bitcoin environment is a disagreement on weather it's safe to introduce non-backward-compatibile changes.  Emails have also evolved, for instance emails with formatted text, images and attachments was unheard of in the old days - though every step is sort of backwards-compatible, older software will simply not show the formatted text, images and attachments.

Some even claims it's important to stick to one client implementation, one server implementation and one central server, so that it's easy to make protocol changes (i.e. Moxie Marlinspike defending signal/OpenWhisperSystems not allowing federation in his article [Reflections: The ecosystem is moving](https://whispersystems.org/blog/the-ecosystem-is-moving/)).  Is a "benevolent dictator" and homogenic software the only way to build a progressive network?  A centralized network without a public open standard can still provide a decent API allowing third-parties to create gateways, alternative clients, etc, and when everything is free software, there is always a safety valve - one can fork off the software and the network if one disagrees with the direction.  Due to the network effect, it's probably never practically possible though.

# Decentralization and federation

In an ideal network there is no central servers or other dependencies on any single entity.  When a single entity controls the servers, said entity may become corrupt, compromised, may die or go bankrupt, etc.  Such dependencies causes fragility.

In the ideal chat network, anyone can start up their own nodes in the network without needing any permissions, no node in the network is more special than others, and people may even chose between different implementations of the node software.  Email works like that.  IRC sort of started up like that, but eventually since any IRC server administrator has full superuser access the model broke down, and only approved servers would be allowed to connect to the network.

There are some big differences between IRC and Email; With email, you register up somewhere, and an email address belongs to a particular server (or cluster of servers) - just like your physical mailbox belongs to your home location.  With email, the server is not actively joining a network - an email server can be standing idle, not receiving emails, and nobody would even know it exists.  With email one typically have to either set up a personal mail server or sign up at some provider and and register an email account.  With email, there is no state stored in the "network" as such; it's up to every user/client to have some kind of address storage/lookup system.

With IRC, a user doesn't belong to any particular server, one can typically connect to any server in the network (oh well, at least in the old days when it was *one* IRC network - now there are quite some standalone and dedicated networks), the servers are actively forming a network, and one usually don't need to do any kind of registration (except choosing a nick handle - and most networks now allows people to "register" the nick, i.e. set a password),  In chat networks there is often significant amounts of state stored in the network, such as who is online and whom is not, adressing information for the various nich handles, registery of public channels/"groups (or topic tags or similar), and often enough contact information on every participant that people can find their friends through real name search, telephone number search or nickname search.

I think that in the perfect chat network quite much such state should be stored in the network itself; long-term information should be consistently stored (if a nick registration fails after ten minutes - probably no big deal, but if you're well-known as BigBoss and has been used that nick for several years, it shouldn't be possible for others to simply steal it), and it should be stored in a decentralized way.  Both servers and internet connections as such can go down.  CAP-theorem says there are three important properties in a distributed system, it's availability, consistency and partition tolerance, one has to chose, one cannot have all three.  With chat networks it's often acceptable to forsake consistency; in IRC one may often have "netsplits", without a centralizied registery of channel and nick ownership it's often possible for attackers to steal channels or nicks during netsplits.  When IRC was at it's peak popularity there was frequent DoS and DDoS-attacks against IRC servers from people that wanted to steal (or reclaim) channels or nicknames.  This is a serious weakness with IRC.  Blockchain-based systems also forsakes short-term consistency (this is the reason why one often has to wait for "three network confirmations" before a bitcoin transaction is accepted; the receiver wants to be very sure that you don't utilize a netsplit to send the same coins to two different addresses), but they are able to preserve long-term ownership without needing centralized databases.  Apparently a good chat system should have some kind of blockchain-based system for storing nicknames and such.

Is it really important with a fully distributed system?  Please leave a comment.

![By Rob Hille (Own work) [CC BY-SA 3.0 (http://creativecommons.org/licenses/by-sa/3.0)], via Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/5/52/Mycelium_RH_%288%29.jpg)

# Final words

With a decentralizated network and open protocols, it should usually be possible to create gateways/bridges for connecting different chat networks, that may be a solution to create one network out of the current fragmented mess.

Are there other points worth mentioning that I have forgotten?  Of course, security is important, and I also have a list of features that a modern chat network should support - but that's for a future post.  Finally I'm intending to compile a list of existing services and how they compare with the requirements.


Do you think any of the above points are more or less important than the others?  Please leave comments!

# See also

* [EFF secure messaging scoreboard](https://www.eff.org/secure-messaging-scorecard)
* [Github repo](https://github.com/tobixen/chat-articles) for those articles
* First and previous article: [The great chat fragmentation](https://steemit.com/technology/@tobixen/the-great-chat-fragmentation)
