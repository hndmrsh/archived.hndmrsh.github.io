---
layout:		blogpost
size:     s
title: 		"Ludum Dare #23: A journal"
excerpt:	|
  A cross-post of my journal kept during Ludum Dare #23, and the development of _trapped._
colour:   "#33B506"
tags: 		game-dev post-mortem
crosspost:
  name:		"samuelhindmarsh.wordpress.com"
  url:		"https://samuelhindmarsh.wordpress.com/2012/05/17/ludum-dare-23-a-cross-post/"
see_also:
  name:		"trapped."
  url:		"/games/2-trapped.html"
---
#### First post from a first comp-er

Well here goes.

I first heard about Ludum Dare during the previous competition, LD \#22. I thought it sounded like a great idea, and enjoyed watching a number of live streams over the weekend. Immediately, I decided that I was going to enter LD \#23, and was pleasantly surprised to learn that it fell during a two-week break from university. But alas, a number of things have since transpired to ensure that my first Ludum Dare would be less than ideal, including:

1. A large number of assignments which need to be completed over the break. One for each of my four courses, in fact. If I can’t get these finished in time, then there will be no entry from me this year. I really don’t want this to happen.
2. The second round of the ANZAC League, the preliminary competition acting as qualifiers for the International Collegiate Programming Competition, is scheduled for Saturday, 20th of April. Including transport, this will take approximately the first seven hours out of Ludum Dare. Not only that, but the competition is mentally exhausting.
3. Turns out the competition is on the last weekend of the uni break, and because of the time difference here in New Zealand, it doesn’t end till 1pm on the Monday. Unfortunately this means submitting my entry on Sunday night.

Combined with work commitments, my sleeping schedule, food intake requirements and A-League Grand Final watching, I’ll have a total of about… 15 hours to work on my entry. Regardless, I am determined to submit an entry for this competition. Due to my very limited time constraints, and the fact that it is my first attempt at the competition, my entry is probably going to be poor at best.

A few details about my entry:

- I’ll be coding in Java – it’s my language of choice, and it’s nice and portable, so anyone which the JRE installed (that should be just about everyone these days!) will be able to play it.
- I’m not an artist, so I’ll probably be knocking up some pretty “abstract” graphics in Paint and making them look a bit flashier in GIMP.
- I’ll be using community-favourite sfxr for sound effects, and if I have time, I’ll be using FL Studio to make some music (and JLayer for Java mp3 support).
- I’ll be making a timelapse using Chronolapse. They’re fantastic, I love watching them!
- Unfortunately, because internet connections in New Zealand are poor (and my 20GB/month data cap – I know!) I won’t be live-streaming. I will be writing the occasional blog post here, however.

After the competition ends, I’ll be cross-posting all the blog posts and the final game on my personal website (which I won’t plug here – it’s pretty bare at the moment!) for archival purposes.

Bring on next weekend!

#### The Day Before:

In my first post, I pointed out that I would be severely limited in the amount of time I’ll be able to set aside for LD23 this weekend, and combined with my complete lack of artistic ability, I’m glad to say that my Minimalism theme has made it through to the final round of voting! I’m obviously hoping it becomes the chosen theme for this LD; it would mean I would be able to get away with Magnavox Odyssey-esque graphics, and call it an “artsy” game, as well as saving me plenty of time I would have otherwise spent on the art.

I spent today drawing a class diagram of one of my previous games, in order to get an idea of how to best set up the underlying engine stuff. I don’t have much history as far as games go, and writing an engine from scratch in a 48-hour game development competition seems frankly self-destructive (I’ve never used any libraries before – I’ll probably learn how to use LWJGL or something before LD24) , so I need all the preparation I can get. It will be a challenge, no doubt.

Hope you’re all getting excited about the weekend – I know I am!

#### All done!:

Successfully completed and submitted my entry with 12 hours to spare!

As I mentioned earlier, I was incredibly short on time this weekend, and had to whip this game up in 11 hours. Combined with the fact that the engine was built from scratch in pure Java (the only library I used was JLayer, for the playing of mp3 files), the quality is a little poor. However, it’s perfectly playable, so that’s something I’m proud of.

LD23 has been a great experience, and definitely one I’ll be able to learn from for LD24. But I’ll discuss that in a proper post-mortem tomorrow.

Good luck to everyone else who’s still going – push hard for these last 12 hours!

#### trapped.: A Post-mortem

I’ve been putting off writing a post-mortem for a while now, so I thought I should really write it before voting closes tomorrow and interest in LD \#23 dwindles. So without further ado…

_What went right:_

- First and foremost, I actually finished a completely playable game. This was one of my main goals, and I’m delighted to have achieved it. The game was not at all deep or involving, but it was simple and it was fairly well polished. As I’ve mentioned before, I was pressed for time over the weekend, and only had at most 24 hours (including sleeping, eating, etc.) to work on the game, so my aim wasn’t set unreasonably high.
- I stuck to what I knew – no testing out new frameworks, languages or programs in a high-pressure situation! – and so I was able to devote the entire time to creating the code and assets.
- Luck! Somehow my collision detection code, something I have normally struggled with throughout my limited game development history, worked almost perfectly first time. Not only that, but my music sounded pretty good, pretty quickly, and even my art assets, as simple as they were, looked half-decent after spending only a few minutes work on them.

_What went wrong:_

- Building an engine from scratch – the epitome of reinventing the wheel. Learning to use a framework like LWJGL before LD \#24 will be a focus for me, as it will greatly reduce the amount of time necessary to get a game going, allowing me to focus more on the gameplay than just being able to play the game.
- Having no ideas prior to the start of the competition. I had my first idea 9 hours into LD \#23 (although the first 9 hours I was spending on another competition anyway), and it ended up being the idea I stuck with just so I could get it a game done in time. The lack of ideas also demotivated me somewhat, so a bit of preparation in this respect before the weekend will allow me to make better use of the limited time next time. One of the best ideas I read was to come up with an idea or two for every one of the potential themes in the final round of voting, so that when the theme is finally announced, you have a bit of a head start.
- Not working around my weaknesses. I mentioned before about how my art assets looked pretty good after spending only a few minutes on them; however, that was true only for the third iteration of the art. My first attempt at the art had me redrawing moderately complex figures and scenery numerous times, before I eventually decided that I would have to go with abstract shapes to overcome my lack of artistic ability. In the end, it ended up looking good, and had I had more time, I would have loved to have tied the story and gameplay into the abstract aesthetics more – for example, the reason the player is red and the enemies white is because I had toyed with the idea of the story tackling the themes of racism and prejudice.

All in all, I felt it was a successful first attempt at a Ludum Dare compo entry, and I can’t wait for LD \#24 – I’ll be looking to make a much deeper game next time, with the story, graphics, music and gameplay creating a cohesive experience. That’s the aim, anyway!
