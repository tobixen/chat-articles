

In this post I'm trying to describe what I want from a chat network.  I'm also planning to try to make a list of existing chat services and see how they compare to the requirements listed here.

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
# Security

## Protection against spamming

In any communication network where people can create new accounts for free and reach out to anyone, spam and phishing is bound to become a problem.

Some ways to prevent it:

* Content filtering - that's one of the ways we've traditionally been using for fighting email spam - but it's a bad idea; the risk of filtering away false positives is always there, "spam filtering" has been used as an excuse for censoring away unpopular opinions in some contexts, and it's an arms race - a skilled spammer would always find ways to get through the filters.
* Blacklisting/whitelisting senders and sender networks - that's also one way we've traditionally been using for fighting email spam, it's also a bad idea, it may cause a centralization pressure, people may find themselves blocked without being at fault, and it can be abused for censorship purposes.  With IPv6, addresses are cheap.
* Cost - a direct monetary cost, CAPTCHA or a [Proof of Work](https://en.wikipedia.org/wiki/Proof-of-work_system)-concept may restrict spamming to some extent - but it's a quite inefficient spam-filter; any kind of cost on sending messages (or registering accounts) will work as a deterrent against some legitimate use-cases, in the same time some spammers may easily eat the cost, the worst spammers may even manage push the cost over onto others.  Proof of work is not a good concept, spammers with access to the right kind of equipment may push out spam at a high rate (t).  perhaps at no cost for the spammer (utilizing resources they have gained unauthorized access to, or just maxing out CPU that they have rented on a flat rate), while users trying to send legitimate messages from old hardware will have annoying delays while the device is trying to send the message - the cost in terms of wasted battery power may be a real problem.  The users are cost-sensitive, too much costs and people will chose other networks.  Captchas are annoying and difficult to set up a good captcha-system that works for the disabled and isn't centralized.
* Some kind of identification of the sender, and blocks on abusive users.  Many modern chat systems uses a telephone number for the identification part; this may work to some extent as it's usually non-trivial to source a big number of telephone numbers cheaply - though it's difficult to authenticate and block users in a decentralized manner, and in reality there is no one-to-one-mapping between people and telephone numbers - some people have 0 personal telephone numbers, others have several, and yet others are frequently changing theirs.  Others may also want to chat anonymously or pseudonymously, without the conversation being tied to a telephone number.
* An invite-only-network, i.e. that one has to give away a public key or a username and a code outside the chat system.  This prevents adoption, so no good.  In some systems one has to establish a connection before one can chat - but it's often possible to abuse the "hi, please connect with me"-message for spam purposes.
* A peer-to-peer online identity and reputation scoring system could probably have solved this nicely.  Actually, I think we really need a global open peer-to-peer reputation scoring system - more about that in future posts.

![By Peter Eich (www.bodenseepeter.de) (Own work) [CC BY-SA 2.5 (http://creativecommons.org/licenses/by-sa/2.5)], via Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/b/ba/Spamfilter.jpg)

## Protection  with encryption also on the meta-data; noone should know that Alice has spoken with Bob.
with good authentication of the sender - it should be impossible to send with a spoofed sender identity ...
 ... but "deniability" may also be an important feature, the sender may not want the receiver to be able to prove that the chat has taken place
with forward secrecy: past communications should be secure even if the keys are stolen
audited: an external party ought to have audited the security design and code
