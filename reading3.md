# Dark UX Design Patterns

Reading the TechCrunch article, I especially found the mentioning of intentional design friction interesting. Design turns evil when the company's interest conflicts with that of the user. If a user doesn't want to consent to certain things, the easiest thing to do is make it harder for them to opt-out.

I actually find Facebook's aquisition of WhatsApp infuriating. WhatsApp's purpose was private, secure communication. People who used WhatsApp used it becuase it was more secure and private than other options. Facebook stepped in and took advantage of those users' trust in order to feed more data into their platform in a move that throws the notion of privacy and ethics out into the wind.

Another major issue is this:

![](https://techcrunch.com/wp-content/uploads/2018/04/screen-shot-2018-04-25-at-1-01-35-pm.png)

Does this make it clear that Facebook uses this facial recognition in order to track what photos you appear in, even when they have no association with your account, in order to track your interactions, cross reference common interests, and target advertising based on how your interests might be similar to your friends'? No, it does not. It manipulates you into opting in for fear of being impersonated. As if that's why Facebook _really_ developed the feature.

One thing I disagree with about the article is the argument it makes about having a brightly colored button and a plain one. If your "opt-out" link is somewhere else nowhere near the highlighted "yes" button (see Windows section below), then this point is 100% valid.

But when done properly, with the opt-out right next to the opt-in, and the opt-in being the one that's highlighted, it complements the user's expectation that the highlighted button is "yes" and the other one is "no." When a screen asks "Do you want to enable this feature?" I believe it intuitively follows that the highlighted button says "yes I do," and the plain one says "no I don't." It would actually be even more confusing to highlight the "opt-out" button, and it would just be annoying if neither were highlighted. Users expect to be able to navigate a screen at a glace, so making them pay special attention to what each button says and will actually do slows things down. Just highlight the "yes," leave the "no" plain, and make sure they're next to each other.

Looking at the thumbnail of the article immediately reminds me of the short-lived [GDPR hall of shame](https://web.archive.org/web/20180623153852/https://gdprhallofshame.com/), a blog which lasted for 22 posts listing examples of shady practices exposed by the EU [General Data Protection Regulation](https://en.wikipedia.org/wiki/General_Data_Protection_Regulation) from 2018.

A few highlights:

 1. [Tumblr presents a list of 322 "partners,"](https://web.archive.org/web/20180611073755/https://gdprhallofshame.com/22-to-continue-to-use-tumblr-please-check-these-2-000-boxes/) each of which has to be _individually_ opted-out with its own checkbox. There's no "opt-out all" button. You need to click/tap 322 times. Oh, and you'll have to do it again when you use it on a different device.

 2. [Zoom email communications "opt-in"](https://web.archive.org/web/20180623153852/https://gdprhallofshame.com/17-zoom-that-isnt-how-consent-works/) isn't really an opt-in. I'll let the screenshot speak for itself.
    
    ![](https://web.archive.org/web/20180623165307im_/https://gdprhallofshame.com/content/images/2018/05/zooooooom.jpg)
    
 3. Perhaps the most ironic is [TechCrunch parent company Oath's response](https://web.archive.org/web/20180528093119/https://gdprhallofshame.com/5-techcrunch-engadget-and-oath-cookie-gore/).
    
    ![](https://web.archive.org/web/20180528093119im_/https://gdprhallofshame.com/content/images/2018/05/1.jpg)
    
    You get presented with a wall of text, which notably says: "Select 'OK' to continue using our products, otherwise you will not be able to access our sites and apps," immediately followed by "Select 'Manage options' to set your data use and sharing choices." After clicking "Manage options," it doesn't get better.
    
    ![](https://web.archive.org/web/20180528093119im_/https://gdprhallofshame.com/content/images/2018/05/2.jpg)
    
    _Again_, we have _another_ generic consent screen that says you have to click OK, and then shows an even smaller link that actually might be something useful.
    
    ![](https://web.archive.org/web/20180528093119im_/https://gdprhallofshame.com/content/images/2018/05/omfg.jpg)
    
    And now we get to see what they were hiding. Literally hundreds of data partners, all of which are opted-in by default. At least there's a "deselect all" button.
    
    If you had selected "OK" on either of the previous screens, as it strongly encouraged you to do, you would have "opted-in" to all of these partners processing data without even realizing it.

---

But all of these pale in comparison to the worst. This is the cracken of software. It makes Tumblr seem private. And it's on over 75% of desktop computers.

### Windows

Windows 10, the $139 propriety software used by over a billion people, has some of the worst practices I have ever seen.

After going through the installation process, _setup_ begins.

The first screen you see is this: [(Credit)](https://www.hardwarezone.com.my/feature-heres-step-step-guide-installing-windows-10)

![](https://assets.hardwarezone.com/img/2015/07/W10install-08.jpg)

Get going fast! Just say "do whatever you want" and get to using your computer faster! Don't bother with those pesky settings and _options_! Send Microsoft and _trusted partners_ your location? Why? Because you want to! See it's the big blue "Express settings" button!

Oh wait you want to actually have control? Where's waldo—I mean where's the customize settings link?

Once you actually find the link, you go ahead and turn off the switches and proceed to the next step. What's next? [(Credit)](https://www.windowscentral.com/how-create-local-account-during-windows-10-home-setup-process)

![](https://www.windowscentral.com/sites/wpcentral.com/files/styles/larger/public/field/image/2019/12/local-account-missing-windows-10-home-fix.jpg)

I need to make a Microsoft account? And _that's_ what I'm going to use to log in to my computer?

Holy hot garbage. This may not seem like a big deal, but consider this:

 1. Your Microsoft account has access to your Outlook inbox, which potentially has the ability to reset _all_ of your passwords.
 2. When you sign in through your Microsoft account, the password you use to unlock your computer is the _same password_ as your Microsoft account.

Why is this a bad idea? Because you're going to be typing your login password _dozens of times a day_. So, by forcing this to be the _same_ as your Microsoft account, Microsoft is (a) _encouraging_ weak passwords that can be typed easily, and (b) allowing any eavesdropper to _easily_ steal your _email password_. Wow.

Seriously, wow. Apple, one of the most controversial anti-consumer companies on the planet, doesn't do this. Sure, they prompt you to sign in when setting up, but they _don't_ reuse the same password to unlock your computer, and more importantly, _there's a skip button_. Seriously, take another look at that screenshot. Is there a skip button anywhere?

So how do you skip the Microsoft account? Well, as Microsoft would tell you, _you don't_.

There is a trick. You can turn off the network connection, and then click on "Create account." The account creation page will fail to load and only _then_ will Microsoft finally grace you with the option to skip.

But here's the kicker: Microsoft _does_ allow you to skip it. Just only if you pay $60 extra. Yes, you need to pay **$200** for Windows 10 Pro to have the _priviledge_ of avoiding this _objectively bad_ feature. For the _luxury_ of setting up your computer the same way you have for _decades_, it'll be a $60 premium on top of the already exorbitant price tag. And once you do, it's still entirely non-obvious. You actually have to select "Join a domain," which makes no sense, and then somewhere there's a local account link.

This is a change Microsoft made _after the fact_. When Windows 10 first came out, there was an option, even though it was much better hidden than the "customize settings" link above, and it repeatedly begged you to change your mind and make an account instead. But it was there. Horrible, still dark UX, but at least an option. [In May 2019](https://www.howtogeek.com/442609/confirmed-windows-10-setup-now-prevents-local-account-creation/), Microsoft _removed_ this feature, forcing users to use the plainly ridiculous workaround of disabling their internet.

---

Oh, and Microsoft requires you to sign your device into an account anyway to use many features like the Microsoft Store. It's true that this is typical among competitors, but at least they don't replace your separate login password with your most cherished and secret one.

Oh wait—

![](https://s14633.pcdn.co/wp-content/uploads/2017/10/chromebook_setup.jpg)

[(Credit)](https://www.bruceb.com/2017/10/how-to-set-up-a-chromebook/)

> PS: Since when is the Mac the last major product to have a good thing?

## Questions

1. How can you ensure that your design is flexible and adjustable enough to be approachable by anybody? How can you identify the issues various people have and fix them? What if focus groups don't reach a broad enough audience? How can you tell that you're not doing enough user research?

2. How do you avoid the slippery slope of the guiding the user to what they want (e.g. if a user already knows they want to use your app, it should be obvious at a glance what they need to do), while trying to avoid pushing the user too hard? How can you "fast-track" the experience to reduce friction, without going pushing the user to go "too fast" so they don't really know what they're getting into?

3. What's in it for the business? Why is dark UX bad for business? How could a UX designer convince upper management that dark UX design patterns are bad for business?
