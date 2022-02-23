# pear-no-s
**Warning: Many screenshots will contain slurs against colored people as well as homophobia and transphobia**

A little introduction: <br>
Pearos is a linux distro based on kde neon (or kubuntu or debian, more on that later), that is made to look as close to macos as possible, it's supposed to be a "successor" to the old pearos, which has been discontinued for some time, the old developer is not affiliated to the new pearos.

## Distribution mismanagement
Pearos is horribly managed, not only does it use a different distribution for the base with almost every release, it seems to switch between debian, kde neon and kubuntu. Not only does this require you to reinstall with **every** new release, but will also cause general management issues as they all have different package versions. <br>
Updating the system with `sudo apt upgrade` would/will destroy your installation by either resetting all themes or removing really _all_ branding of pearos, turning it into a kde neon/kubuntu/debian installation. <br>
<br>
## Not paying the host
They use a third party host for the isos(they call it a cdn even though it isn't one), which obviously costs money, however they just [didn't pay](https://github.com/axtloss/pear-no-s/blob/main/images/wontpay.png), they excused it with that they ["don't have money" and have to pay for "other stuff"](https://github.com/axtloss/pear-no-s/blob/main/images/donthavethemoney.png) and also got very pissed off when the person who owns that host said they'd [terminate it if they wouldn't pay in 2 days](https://github.com/axtloss/pear-no-s/blob/main/images/paidotherhost.png). (they had to pay ~2.70GBP, which I kinda expect everyone to have, but we'll give them the benefit of the doubt for now), so if they really don't have the money, they just shouldn't have used the third party host.<br>
However they then did [pay after it got suspended](https://github.com/axtloss/pear-no-s/blob/main/images/paidotherhost.png), meaning they do have the money.
## License issues
Pearos has a virtual assistant built into it, called "Piri", the backend of that [was made by me](https://github.com/axtloss/vAssistant), at first we had a special License agreement that allowed them to use my backend if they put credit in the application. However, when I published the code on github I changed the license to gplv3 and also properly told them about it. However, it took a **long** argument to make them also open source the piri source. After some they just wiped the repo and started everything again, still using my backend, but they didn't put back the gplv3 license and went without any license. I then updated the license to the nolicense v1 and they didn't update it either. After I told them about it (I've left pear since a very long time by that) they got very pissed and started mentioning "my weird license addiction". In the end they privated the original piri and made a a custom one.<br>
<br>
They use the macos icons and are making money off of it, I think that's self explanatory.<br>
<br>
### Neofetch
What's a distro without proper representation in neofetch. The proper way to get your logo in neofetch is by forking neofetch, adding your distro and then opening a pr to upstream with that ascii. <br>
Instead, and I have to admit I could've done it better myself, alexb asked me to create a custom neofetch that has the pearos logo and some extra visual changes, as well as a directly printed copyright message. This message was still there until one release after I left pearos (monterey), in nicecore, alexb just removed my name from that copyright message and left his name there: <br>
Left shows the pearos nicecore neofetch and right the monterey neofetch
![Left shows the pearos nicecore neofetch and right the monterey neofetch](https://github.com/axtloss/pear-no-s/blob/main/images/neofetch.png?raw=true)
This obviously is not ok since I'm the original author of that modified neofetch (not to mention that the mit license with dylan's name is still in the source).
<br>
### Pearos-arch
Alexb is trying to release pearos based on arch again, which isn't an issue in itself, except that all the build scripts and arch configuration is copied from [archlinux gui(here also referred to as "alg")](https://github.com/arch-linux-gui), without ever mentioning that the code was taken from archlinux gui in the readme or code(not even making the pearos arch repo a fork of archlinux gui). Some examples:
- [The hostname is archlinuxgui](https://github.com/axtloss/pear-no-s/blob/main/images/pearos-arch-copied/alg-hostname.jpg)
- [Package list also seems to be copied from alg](https://github.com/axtloss/pear-no-s/blob/main/images/pearos-arch-copied/alg-packages.png)
- [Using alg repos](https://github.com/axtloss/pear-no-s/blob/main/images/pearos-arch-copied/alg-repos.png)
- The copyright header on all files (`SPDX-License-Identifier: GPL-3.0-or-later`) appears on the same point and files as in the alg files. [But also uses the pear license for other stuff?]()
<br>

## Violation of GDPR
In the website https://pearos.xyz/ they show a button for the privacy policy, which is needed by for-profit companies (pearos is one since they do make money), however when clicking on that, it leads you to https://privacy.pearos.xyz/ which you can't access because it returns a 403 nginx error. That means that pearos doesn't show the user any privacy policy. Which violates the gdpr.
<br>

## Bigoted dev
This is the biggest reason to not use pearos (in my opinion)<br>
**Warning: This part will contain screenshots with various slurs, the screenshots will be hidden, unless you actively click on the links to images.**<br>
The main dev and "founder" of pearos is a huge bigot.<br>
- [He actively uses the n-word](https://github.com/axtloss/pear-no-s/blob/main/images/n-words/Use%20of%20n-word.png)
- [He activerly uses the n-word part 2](https://github.com/axtloss/pear-no-s/blob/main/images/n-words/Use%20of%20nword.png)
- [Finds transphobic "memes" funny](https://github.com/axtloss/pear-no-s/blob/main/images/transphobic_meme.png)
- [Uses a transphobic slur in piri (I'll talk about this a bit more)](https://github.com/axtloss/pear-no-s/blob/main/images/trans-slur.png)
- ["Gay is an offensive word for homophobes" -alexb](https://github.com/axtloss/pear-no-s/blob/main/images/gay%20is%20offensive%20for%20homophobes.png)
- [In the discord server they have a running "joke" about using nice car and spoilering the "ce ca" part to make it look like they said the n word](https://github.com/axtloss/pear-no-s/blob/main/images/nicecar.png)
- [Used the n-word in a script shipped in pearos Cupertino](https://github.com/axtloss/pear-no-s/blob/main/images/n-words/nword-in-script.png), it's in `/usr/share/extras/pear-map-plymouth/install.sh` you can view this file on pearos cupertino 20.09, (available on archive.org), [this is what it looks like when executed](https://github.com/axtloss/pear-no-s/blob/main/images/n-words/n-word-in-script-executed.png)
- [Deadnamed me](https://github.com/axtloss/pear-no-s/blob/main/images/deadnaming.png)
- [This whole thing](https://github.com/axtloss/pear-no-s/issues/2) in which he
  - deadnames me
  - uses their trans service provider as an excuse as of why he's not transphobic
  - Makes a transphobic joke <details> <summary> CW:: Transphobic joke </summary> "Why did you assume my gender? (that question is with humouristic purposes, I go by hell/boy. Jk again, I go as he/him. For real" </details>
  - After being told by multiple trans people that "s\*\*\*ale" is a transphobic slur, he still [looked up what it means to prove me wrong](https://github.com/axtloss/pear-no-s/issues/2#issuecomment-1032974828)
  - [Tries to justify deadnaming](https://github.com/axtloss/pear-no-s/issues/2#issuecomment-1032977894)
  - [Quotes a law that doesn't even apply to me](https://github.com/axtloss/pear-no-s/issues/2#issuecomment-1033466894), and trying to use scare tactics on me(mind that I'm a minor), to get me to not be silent
  - Tries to justify Racism/using the n word "In Balkans we don t share the same racism obsession, for Balkan people it is JUST a word" [as well as this](https://github.com/axtloss/pear-no-s/blob/main/images/n-words/justifynword.jpg)(for context, I found the nword in the script mentioned before and asked him about it, he tried to justify it like that)
  - The fact that "My opinion 'bout LGBT people and black people" exists in https://github.com/axtloss/pear-no-s/issues/2#issuecomment-1032915921
  - and much more (read through the issue and you should see them)
- [Makes jokes against disabled people](https://github.com/axtloss/pear-no-s/blob/main/images/jokeagainstdownsindrome.png)
- [Makes an "All lives matter" joke as a response to me mentioning the point above](https://github.com/axtloss/pear-no-s/blob/main/images/windowmanagerlivesmatter.jpg)
- [Uses black emojis(he is not black) and then says "oh wait is using black emojis also offensive", in a mocking tone](https://github.com/axtloss/pear-no-s/blob/main/images/blackemojis.jpg)

## Transphobic slur in piri 
This one is a special case, originally There was a [post on r/unixporn (has been deleted)](https://www.reddit.com/r/unixporn/comments/mqd9q2/plasmamom_can_we_have_macos_at_home/) <br>
And then there was this comment [CW: contains transphobic slur](https://www.reddit.com/r/unixporn/comments/mqd9q2/comment/gufyq5b/?utm_source=share&utm_medium=web2x&context=3) <br>
It was true, Alexb included a slur in piri. I contacted him about that and told him to remove it and he supposedly did. But with the release of pearos monterey (after the https://www.reddit.com/r/unixporn/comments/mqd9q2/plasmamom_can_we_have_macos_at_home/ thing has happened), look what I found: <br>
[CW: transphobic slur](https://github.com/axtloss/pear-no-s/blob/main/images/trans-slur.png)
This one really annoys me because it's really just disrespectful, he includes a transphobic slur in an application of which the backend was made by a trans person. Not only did he _lie_ to me and others about having it removed, he also just continued including it in newer releases and didn't even patch it from the release that was the newest during that time. <br>
<br>
___
<br>
Those are all the reasons you shouldn't support/use pearos. It's a terrible experience, the main dev is a huge bigot and doesn't care about licenses
If you're wondering why you should trust me with what I said, I used to be a dev for pearos, I've made the backend for the pext installer and also developed many of the pexts. <br>
If you have other points I could add you can create a new PR or open an issue and I'll include them. <br>
For questions you can ofc open an issue. Any type of disrespectful comments (I sorta expect them because of the last topic) will be deleted. 
