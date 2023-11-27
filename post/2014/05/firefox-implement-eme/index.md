---
title: "Why I think Firefox SHOULD implement EME"
date: ""
categories: 
  - "blogs"
tags: 
  - "firefox"
coverImage: "mozilla_firefox_logo.png"
---

_As you might've read on the internet before now, Firefox will implement EME(**Encrypted Media Extensions**). While the internet is in uproar about this, I think they do not have a choice._

### What is EME

EME is a JavaScript API to play encrypted media. This would mainly include videos. You can think about encrypting Netflix and Youtube video's. With this, they should be able to protect copyrighted materials.  For this, the browser needs an extension to communicate with a license server to get keys to enable decryption of the media.

When talking about Netflix, a usage could be that EME would authenticate you as a user, determine your identity and permissions and decide if you're able to decrypt the file and play it.

The decryption is done by the Content Decryption Module. This is a client side or hardware module. It receives a license from the License (Key) Server and eventually decrypt and decode it.

### Other browsers

Firefox will not be the first to include EME. Internet Explorer 11, Chrome, Safari, Opera and probably some other browsers have already implemented it. Not everyone liked it, but sadly, they have to.

### Why they need to

While most people don't want EME, Mozilla can't just ignore it. When they would, users will eventually not be able to view some media. Other sites may even block Firefox from their sites just to protect themselves. Most users won't temporarily switch to another browser to view one site. If one browser supports most, excluding a few sites the user wants to visit and the other supports them all, the user will switch.

There are some users who will stick to a browser, I've seen that with Opera in earlier versions of the browser. Some sites just blocked Opera by showing them a message that the user cannot view the site with Opera and that they should switch to a "decent" browser like Firefox.

This means, for me, that I'm not mad. I won't stop using Firefox. Firefox has resisted it as long as they could, but what are the alternatives? Do you protest by switching to another browser? Well, you're out of luck then. The other mayor browsers have already implemented it before... EME is here and it seems like it's here to stay.
