# Zev Eisenberg

I quickly became fascinated by the way [BlindWays](https://www.raizlabs.com/blog/2016/12/altconf-2016-user-centered-approach-solving-micronavigation-blind/) works with built-in device features to create an accessible experience for blind people.

There three design elements that I noticed immediately when he showed the app:

![](https://is2-ssl.mzstatic.com/image/thumb/Purple113/v4/c5/63/e5/c563e58b-0469-214d-42a6-b92cc4055122/pr_source.png/300x0w.png)

> The layout of the app is stacked linearly. It doesn't use columns, grids, or other non-linear layout. This allows someone using VoiceOver to drag their finger down the phone screen to easily get all of the information, without having to worry about searching the entire surface of the screen.

![](https://is4-ssl.mzstatic.com/image/thumb/Purple113/v4/28/00/5b/28005baa-1861-0bf8-ca3b-e47b7742951d/pr_source.png/300x0w.png)

> By providing a common frame of reference and mitigating the need for user-provided phrasing, the app doesn't actually remember exact directions or clues. Instead, it simply remembers a handful of landmarks and their position relative to the bus stop, and uses that to dynamically generate clues that make sense from the point of view of the walker. "There is a fire hydrant in front of the bus stop" is much more useful than "There is a fire hydrant south of the bus stop."

> Moreover, worrying about frame of reference can be potentially confusing to someone trying to write the clues. BlindWays solves this using a cleverly-designed visual screen, so it feels less like describing relative positions and more like selecting a spot and picking what should go there.

Finally, and I don't have a screenshot to show this, but BlindWays doesn't try to reinvent the wheel. As a developer making an app for the blind, I might have the intuition that I should build in a screen reader, but this would result in a bad user experience. The user is already used to using VoiceOver, VoiceOver has had decades of development across macOS and iOS by a trillion-dollar company, and as iOS gains more accessibility features, these automatically get incorporated into the app without any work from the app developer. Not to mention the effort that would normally go towards the screen reader can go instead to developing the other features of the app.

In cybersecurity, the saying goes "don't roll your own crypto" because you'll just mess it up. Even Sony [incorrectly implemented an algorithm](https://en.wikipedia.org/wiki/Elliptic_Curve_Digital_Signature_Algorithm#Security) creating a massive security flaw. The same goes for accessibility. All you need to do is make sure your UI elements are labelled properly, so the device can understand how your app works, and just leave the rest to the people who know what they're doing.

---

There are three limitations with BlindWays that I noticed. This is no fault of the app, it was designed this way on purpose, but I started thinking about how BlindWays could be expanded:

 1. BlindWays is only applicable to bus stops. If a blind person wants directions to walk from point A to point B, they're still stuck with basic "in 100 ft turn left" directions.
 2. BlindWays is limited in the service area. It only works within the Massachusetts Bay Transportation Authority.
 3. BlindWays relies on croud-sourced landmark information. This means that A) information can be outdated, B) it's not generalizable. It's difficult to get landmark information from GPS data, hence the crowdsourcing. But if there was away to help the blind navigate based solely on GPS directions, then it would greatly expand the scope of the app.

I've started thinking about an app that uses a different device feature for directions: haptic feedback. Modern devices can very precisely "tap" a device the user is holding. My idea is that an app could use taps to signal the user which way to walk. When they're walking on a path, the device can tap at a constant rate (perhaps 1/second) to remind the user they're going in the right direction. When there's a turn, a double-tap indicates a significant change in direction. A triple-tap can indicate a road crossing. At that point, regular tapping pattern will go faster when the user is facing the wrong direction, and gradually slow down as they aim the device, so they can find the correct direction to walk. This is much less ambigious than a simple "left" or "right."

Anyway, I'm still developing the idea, but once I'm done writing this, I'm going start developing a prototype to see if this idea works in practice.
