I touched base on the history of chat networks and problem of siloization in my previous post [The great chat fragmentation](https://steemit.com/technology/@tobixen/the-great-chat-fragmentation).  In this post I'm trying to describe what I want from a chat network.  I'm also planning to try to make a list of existing chat services and see how they compare to the requirements listed here.

A perfect chat service should be ...

* Free
  * free to use - in all aspects of the word "free" ...
  * ... but it's still needed with some protection against spamming
  * possible to use for anyone, on any platform
  * based on free and open source software
  * based on open standards
  * decentralized - not dependent on a single entity (company or person)
  * federated; anyone should be able to set up servers and become part of the network
* Secure
  * encrypted, with strong end-to-end-encryption as default.
  * with encryption also on the meta-data; noone should know that Alice has spoken with Bob.
  * with good authentication of the sender - it should be impossible to send with a spoofed sender identity ...
  * ... but "deniability" may also be an important feature, the sender may not want the receiver to be able to prove that the chat has taken place
  * with forward secrecy: past communications should be secure even if the keys are stolen
  * audited: an external party ought to have audited the security design and code
* Feature-rich ...
  * easy to use for most of us.
  * with possibility for textchat, voice calls and video calls
  * with possibility for both private two-party conversations and group chats.
  * with permission for anyone to set up new groups - instantly.
  * with a public, easily searchable directory of public groups.
  * with decent handling of links, possibility to embed multimedia, rich formatted text, etc

Anything I've forgotten here?  Please do use the comments field ...

Lets go through those features/requirements ...

# Freedom

![Drawn by author, released as Public Domain](http://github.com/tobixen/chat-articles/blob/master/liberatechat.png)

## Free as in gratis - no cost

One is often regarded as a miser if one is reluctant to pay and demanding that some service should be free.  The old phone network and SMS'es are paid services.  There are certainly benefits with this - one should perhaps expect higher reliability and availability from a paid-for service than for some free service, it's to some extent working as a deterent against spamming (but maybe not so much - I do get a decent amount of spam both to my physical paper-mailbox as well as to my telephone), it may cause better utilization of resources ... and it does require resources to build and maintain a perfect chat service - someone has to pay, directly or indirectly.  There ain't no such thing as a free lunch.  Actually I wouldn't mind paying a bit for a decent chat service, except, if it wasn't for ...

* It pretty much has to be gratis to be able to compete in todays market.  Prices for voice calls and SMSes are on the way down, and flat-rate billing plans with unlimited voice and SMSes aren't unheard of today.
* In a complicated network (i.e. the telephone network!) distribution of income among the different providers involved in setting up a connection may be a hard nut to crack - billing and cost counting may be a big cost driver by itself.  An ideal chat-service is decentralized, based on open source and with lots of contributors - in such an environment it can be difficult to collect, process and distribute an income.
* Metered usage payments for a service where the actual cost of usage is insignificant may be bad, as it causes "customers" to spend energy figuring out stupid ways to save money (anecdotes from the real world: telephone-based protocols where information is encoded in the number of rings before the caller hangs up, SMSes without spaces but using capital letters for marking the word boundaries, some russian telecom provider did allow people to call internationally for ten seconds without billing - causing some customers to make hundreds of calls muttering some few words on every call).  Actually, for chat services it can often arguably be a good thing that the sender thinks three times before sending the message - the sender is quite often significally underestimating the time costs of writing the message, as well as context-switching and reading the message on the other side.
* It's also important to consider the income inequities - in some parts of the world a cup of coffee from a café can cost as much as 10 mBTC, and most people finds it affordable - in other parts of the world, 90% of the population makes less than 10 mBTC pr day, and it would be madness to waste a days salary on one cup of coffee!  A price per message that seems really insignificant for some of us may be deemed so expensive that others are excluded from the network.

Would you use a paid-for chat service?  Feel free to tell in the comments :-)

## No evil plans for future profit generation

A service may be "gratis" without really being free - and those services may actually be the worst, I think it's better with honest, up-front payments than service providers giving away services for free and having some secret, potentially evil plans on how to turn it into a future profit.  It's not unusual that a service requires people to read through and accept a very long end user agreement - almost nobody actually takes the time to read through all of it, and often the text contains things that no sane person actually would agree on.

It's not unusual that service providers collect all kind of personal information, even scouring through the conversation content and sell it to third parties, eventually bombard the user with targeted commercial ads.  Being bombarded by targetted commercial ads may by some be seen as a good thing, targetted spam is at least more relevant than random spam - but remember, for someone to send targetted spam on a chat network, they would need to analyze all sorts of private information.  If you just shrug and think that's ok, then I recommend reading the [scroogled](http://blogoscoped.com/archive/2007-09-17-n72.html) short story.  Another anecdote, there was a story about a banking/insurance company buying up a popular supermarked chain (Tesco in the UK if I remember correct), and someone did a bit of research into what kind of insurance offers one would get with and without a Tesco frequent shopper bonus card.  Apparently the shopping history mattered a lot; people with a "healthy family shopping pattern" got quite good discounts compared to customers without a shopping card, people who frequently bought beer and cigarettes got a worse quote.  Consider that some kinds of insurance may be mandated by law (i.e. auto liability insurance) ... next thing, insurance companies doing data mining on your private chat history before giving you an offer.  Is that OK?  I think not ...

Even untargetted marketing ads may be considered evil.  It's annoying, and among other things it may consume expensive bandwidth, precious battery power and the purpose of the marketing is to get YOU to spend money on things you probably shouldn't be spending money on.  A service cannot be considered "free" it it's not free from marketing ads - though arguably financing stuff through marketing ads may be more fair towards the have-nots than financing stuff through usage fees.

How do you feel about services financed through promoted contents on the internet?  Feel free to tell in the comments :-)

## Possible to use for anyone, on any platform

This is quite important, I'd say - a service that can be used by 99% of the population is simply not good enough.  People are often biased, not seeing the inherent restrictions there may be on a product, here are some examples:

* Maybe some 98% of the adult population has a personal telephone number and a mobile phone, but a perfect chat service should cater for 100% (even including children), not only 98%.  Some chat platforms are using telephone numbers as identifiers and text messages as authentication method.  It's all fine and dandy for most of us - but then again, there are people who denies using cellphones for various reasons, so this is no good.  A service using telephone number as identifier should at least provide some workarounds.

* Other chat platforms may provide an android app and an iPhone app - and maybe even an app for the windows phone.  Everyone has one of those three anyway, right?  Wrong!  And even if it was true ... among those that are using those platforms, there are people who couldn't afford upgrading the phone for some years - stuck with old hardware and probably also an old version of the operating system, and probably the latest version of the app won't work anymore.  People like me (SailfishOS - but it does support android apps) may also have a strong desire to be able to do chatting from the laptop or desktop computer.  (Generally, things have improved quite a lot over the last decade - but earlier I would quite often find myself excluded because I run Linux instead of Windows, and generally don't use any Microsoft products at all).

* A bit similar, a chat platform based exclusively on a desktop application or an advanced web application may not work at all on mobile devices.  A person sitting by the computer screen all day may not think about this restriction.  (Generally things have improved during the last decade, earlier quite many web pages was optimized for screens with resolution 800x600 - anything smaller and the web page would be hard to navigate and read, anything bigger and it would look very ugly).

* A perfect chat system should be possible to use also for people with different kinds of impairment.  Yes, doing a text chat with the visually impaired is fully possible - there are specialized software for translating the screen content to spoken text, but if the only available chat client is some complicated GUI client and no text user interface client exists it may be difficult to operate.  Doing a voice chat with someone that can't hear is slightly more difficult.  At least here in Norway there was (is?) a government-paid service with human translators working as a gateway between the old telephone network and specialized text chat terminals for the hearing impaired.  Today I think it's better to just use text chat from end to end.

Is this nonsense?  You probably only need to chat with the 98% normal people out there, and not those other freaks?  Feel free to tell in the comments :-)

## Free and open source software

I'm almost exclusively using [open source and free software](https://en.wikipedia.org/wiki/Free_and_open-source_software).  What's in it for me?  Quality and freedom.

Quality: It used to be a common perception that proprietary closed-source software products had the best quality, backed by well-funded companies with professional programmers and good software development processes - while the free products was flimsy hobbyist projects.  This may have been the truth in the 80s and early 90s, but nowadays it's often quite the opposite, open source products tend to excel on everything except marketing.  It's not so that one automatically gets quality by chosing open-source products - one has to do some due diligence and chose products wisely - but at least one has the chance to do due diligence!  I usually spend some few minutes "peeking under the bonnet" to see if the code looks sane or not. In most open-source projects one can follow the development process carefully - it's like having a look into the kitchen of the restaurant before deciding if it's a good place to eat.

Freedom: It rarely happens that I'm getting my hands dirty and actually do modify open source software products - but it happens.  If something doesn't work as intended for me, or if I want to use the product for other purposes than what the original creator intended, then I'm free to fix things.  If I can't do it due to constraints on my time or skills, then I can pay someone to do it for me.  It's quite trivial to offer a bitcoin bounty for whomever fixes a feature, I can ask anyone on the market ... while with unfree software I'm totally dependent on the company that developed the software.  If the company goes bankrupt or decides to can the product ... though luck.

I could write a lot about why I have a very strong preferance for free software, maybe there will be another post some day.  Do you think it's unimportant?  Feel free to tell in the comments :-)  

## Open standards

It is important that one is free to create other products to connect to the network - it may be competing client, complimentary software, software made for some particular device, for the impaired etc.  One may want to create gateways for connecting different chat-networks or services sending relevant notifications to a group or an individual, etc.  To allow this, it's important that the standard (aka protocol) is well-defined, and it's important that there are good frameworks for improving the standard and resolving conflicts.

Particularly the latter may be important; [IRC](https://en.wikipedia.org/wiki/Internet_Relay_Chat) lost it's network effect because some of its administrators couldn't agree on how to develop the standard (as I've touched upon in [The great chat fragmentation](https://steemit.com/technology/@tobixen/the-great-chat-fragmentation) and that usage and reliability of email has stagnated because it's too difficult to evolve the standard.  [Bitcoin](https://en.wikipedia.org/wiki/Bitcoin) may also be in serious trouble - I've touched on how bad the environment has become on Reddit in [The big Reddit Bitcoin schism](https://steemit.com/bitcoin/@tobixen/the-big-reddit-bitcoin-schism), but the issue at hand is disagreement on what direction the protocol should be evolved in.

Some may even claim that the system has to be centrally controlled so the protocol can evolve faster (i.e. Moxie Marlinspike defending signal/OpenWhisperSystems not allowing federation in his article [Reflections: The ecosystem is moving](https://whispersystems.org/blog/the-ecosystem-is-moving/)) - the IRC and Email has declined and become less usable because it's so very difficult to change the standard - maybe Bitcoin also will go that way.  Is a "benevolent dictator" and homogenic software the only way to build a progressive network?  A centralized network without a public open standard can still provide a decent API allowing third-parties to create gateways, alternative clients, etc.

## Decentralization and federation

In an ideal network there is no central servers or other dependencies on any single entity.  Such a single entity may become corrupt, compromised, may die or go bankrupt, etc.  Such dependencies causes fragility.

In the ideal chat network, anyone can start up their own nodes in the network, no node in the network is more special than others, and people may even chose between different implementations of the node software.  For instance, the old email system works like that.  IRC sort of started up like that, but eventually since any IRC server administrator has full superuser access the model broke down, and only approved servers would be allowed to connect to the network.

Is it really important with a fully distributed system?  Maybe I'm overdoing?  Please leave a comment.

# Security

## Protection against spamming

In any communication network where people can create new accounts for free and reach out to anyone, spam and phishing is bound to become a problem.

Some ways to prevent it:

* Cost - a direct monetary cost, CAPTCHA or a [Proof of Work](https://en.wikipedia.org/wiki/Proof-of-work_system)-concept may restrict spamming to some extent - but it's a quite inefficient spam-filter; any kind of cost on sending messages (or registering accounts) will work as a deterrent against some legitimate use-cases, in the same time some spammers may easily eat the cost, the worst spammers may even manage push the cost over onto others.  Proof of work is not a good concept, spammers with access to the right kind of equipment may push out spam at a high rate (t).  perhaps at no cost for the spammer (utilizing resources they have gained unauthorized access to, or just maxing out CPU that they have rented on a flat rate), while users trying to send legitimate messages from old hardware will have annoying delays while the device is trying to send the message - the cost in terms of wasted battery power may be a real problem.  The users are cost-sensitive, too much costs and people will chose other networks.  Captchas are annoying and difficult to set up a good captcha-system that works for the disabled and isn't centralized.
* Blacklisting of IPs belonging to spammers.  Not a very viable option, particularly with IPv6.
* Some kind of identification of the sender, and blocks on abusive users.  Many modern chat systems uses a telephone number for the identification part; this may work to some extent as it's usually non-trivial to source a big number of telephone numbers cheaply - though it's difficult to authenticate and block users in a decentralized manner, and in reality there is no one-to-one-mapping between people and telephone numbers - some people have 0 personal telephone numbers, others have several, and yet others are frequently changing theirs.  Others may also want to chat anonymously or pseudonymously, without the conversation being tied to a telephone number.
* An invite-only-network, i.e. that one has to give away a public key or a username and a code outside the chat system.  This prevents adoption, so no good.  In some systems one has to establish a connection before one can chat - but it's often possible to abuse the "hi, please connect with me"-message for spam purposes.
* A peer-to-peer online identity and reputation scoring system could probably have solved this nicely.  Actually, I think we really need a global open peer-to-peer reputation scoring system - more about that in future posts.

## Protection  with encryption also on the meta-data; noone should know that Alice has spoken with Bob.
with good authentication of the sender - it should be impossible to send with a spoofed sender identity ...
 ... but "deniability" may also be an important feature, the sender may not want the receiver to be able to prove that the chat has taken place
with forward secrecy: past communications should be secure even if the keys are stolen
audited: an external party ought to have audited the security design and code
