# What are the best layouts that are midish-to-lowish alternating, highish roll, and matching other idiosyncratic criteria?

Under construction @ 2026-02-04 17:09 ...

- [Intro](#intro)
- [Hardware (and software)](#hardware-and-software)
- [Criteria](#criteria)
- [The winners](#the-winners)
- [Runner up](#runner-up)
- [Context](#context)
- [Analysis - overview](#analysis---overview)
- [Analysis - ways of speaking](#analysis---ways-of-speaking)
- [Analysis - keycraft customisation](#analysis---keycraft-customisation)
  - [Layout customisation](#layout-customisation)
  - [Weights file customisation](#weights-file-customisation)
  - [Corpus](#corpus)
- [Analysis - the stats](#analysis---the-stats)

## Intro

What are the best layouts that are midish-to-lowish alternating, highish roll, and matching other idiosyncratic criteria?

Answering that is part of trying to move away from a traditional row staggered qwerty keyboard, which is infamously awful to type on for historical reasons, to find a hardware, software, and layout solution to make typing feel smooth and joyful. Smooth and joyful above even speed improvements. While a more optimal hardware and software solution is likely to make one, with practice, type faster; the overarching goal of "smooth and joyful" is primary.

This article comes out of discussion at the Discord Server [Alt Keyboard Layouts](https://discord.com/channels/807843650717483049/823046923523063818) (AKL).

## Hardware (and software)

On the hardware (and software) side I've settled on a [ZSA Voyager](https://www.zsa.io/voyager), a programmable custom keyboard that has several features, some commendably "opinionated", that make it worth the purchase (I'm not affiliated with ZSA):

* The keys are swappable.
* You can program multiple layers.
* You can program multiple layers through:
  * An easy to use GUI called [Orxy](https://configure.zsa.io/voyager/layouts/YRYG4/latest/0); or
  * Directly customize the underlying (open source) QMK firmware where Orxy is limited; or
  * Use both and merge the result. See [Using a DIY tool to add custom QMK features to your Oryx layout](https://blog.zsa.io/oryx-custom-qmk-features/) by Pierre Poulain.
* It has 51 keys, more than many other programmable custom keyboards, that often go for fewer keys at 42 or 36 keys. As with the [Corne 42 LP](https://keebmaker.com/products/corne-low-profile?variant=47647202410795) or the [Corne 36 LP](https://keebmaker.com/products/corne-36-lp-keyboard).
* It has four thumb keys rather than six thumb keys. Having, and designing for, only four thumb keys seems like the right "opinionated" (and therefore risky) design choice to make using one's thumbs simpler.
* The keycaps are low profile. My personal preference.
* The keycaps have shine-through RGB lighting.

There are more radical recent keyboard designs - see Ben Vallack's demo of the Svalboard @ [I Tried the World's MOST COMFORTABLE Keyboard](https://www.youtube.com/watch?v=-Lz_FNoYHNM) - that are worth consideration. But from among the less radical programmable keyboards - where you have a plane (or two) of keys to hit with the pads of your fingers (and sides of your thumbs) - I commend the Voyager.

More significantly, the rest of the article will focus on the issue of which main layer (a "layout") to use on a less radical programmable keyboard, on a Voyager, or Voyager-like keyboard.

## Criteria

So we are after a layout that is midish-to-lowish alternating, highish roll, and matches other idiosyncratic criteria.

The other idiosyncratic criteria include:

* **Colstag** (column staggered) layout. As colstag is an improvement on rowstag.

* Excluding thumb **alpha layouts**. To keep the thumb keys for other things like backspace, tab, enter, space.

* Must have **bottom row symbol slots** on at least ring and middle fingers. Because I'm set in my qwerty ways for "," and "." (but allow this could be on the left hand).

* Optimising the (main) layer for **general English**.

  I'm wanting to optimise my *keyboard* for typing both general English (prose, essays, etc.) and programming. The ideal corpus of words (excluding symbols) in programming will be different from ideal corpus of words (excluding symbols) in general English. E.g. The keyword "String" is going to appear more frequently in programming. However, the main speed and smoothness impediment in programming are the symbol keys. I'll be taking care of symbols largely with a separate symbols layer; with some high frequency general English symbols on the main layer (chiefly ".", and ","). And so, for the main layer (what this article is about) I'll:

  - Optimize for general English words over programming words; and
  - In my analysis I'll remove symbols from the candidate layouts. Allowing that one's preferred symbols can be inserted in after analysis. And treating symbols optimisation as a separate consideration.

* No **magic key**. As this would make the layout advanced (for me).
* No **repeat key**. As I don't think I'd prefer this over just tapping the relevant key twice; or this might be an advanced (for me).
* Consistent with the above otherwise trying to find the layouts that score best on **the metrics overall**. Noting if you optimize for one metric that can penalize one or more other metrics.

## The winners

My abbreviations:

- "cs" for "colstag", a column staggered keyboard.
- "ns" for "no symbols". That is, symbols where removed from the layout before that part of my analysis that used the analyser [keycraft](https://github.com/rbscholtus/keycraft).
- "~" (tilde) means no key, not the tilde key. Following keycraft convention.

On my analysis, and using the criteria, the winning layouts are:

**ints-cs-ns** by Tanamar. A "3roll" layout.

```
f o u m j  q g d p ~
h a e r x  v s t n i
z ~ ~ l w  y c k b ~
```

(See the angle modded version with symbols at [https://github.com/samuelxyz/layouts#ints](https://github.com/samuelxyz/layouts#ints))

**wave2-cs-ns** by ec0. A "Highish Roll; midish redirect (STRD/SRTD/SRTC)" layout.

```
v l d m ~   z f o u j
s r t c y   b n a e i
q x k g w   p h ~ ~ ~
```

(See the angle modded version with symbols at [Keyboard Layout Document > Chapter 16: High roll-mid redirect layouts > ... > STRD / SRTD / SRTC](https://docs.google.com/document/d/1W0jhfqJI2ueJ2FNseR4YAFpNfsUM-_FlREHbpNGmC2o/edit?tab=t.vb3u6rdlmxg1#heading=h.9ms661dgth73))

## Runner up

**sturdy-cs-ns** by Oxey. Highish Roll; lowish redirect (STRD/SRTD/SRTC)

```
v m l c p  x f o u j
s t r d y  ~ n a e i
z k q g w  b h ~ ~ ~
```

(See the colstag version with symbols at [https://oxey.dev/sturdy/index.html](https://oxey.dev/sturdy/index.html))

## Context

This is a follow up post to my [Regard for inrolly2](https://discord.com/channels/807843650717483049/1439184823615885332/1439184823615885332) which turned into a thread with good feedback on good alternative layouts in general.

I'll repeat my situation as I mentioned it there (with a different emphasis and some addition here):

* I'm a new alternative layout user.
* I've learnt Graphite to about 20wpm on my ZSA Voyager.
* I've read @ec0's [Keyboard layouts doc (3rd edition)](https://docs.google.com/document/d/1W0jhfqJI2ueJ2FNseR4YAFpNfsUM-_FlREHbpNGmC2o/edit?tab=t.2yb5bwiy1wa8#heading=h.rwlzs0nuaefi) (KLD), a distillation of the wisdom of the *Alt Keyboard Layouts* (AKL) community.
* I've skimmed [https://layouts.wiki/](https://layouts.wiki/). In particular, [https://layouts.wiki/guides/start/recommendations/](https://layouts.wiki/guides/start/recommendations/)
* I had come to suspect I dislike highish alternation and like high rolls, especially 3rolls. Something Graphite lacks. That suspicion has been deepened from my analysis.

## Analysis - overview

"My analysis" here means:

1. Taking a long list of candidate layouts to evaluate. Largely those flagged by anyone in "Regard for inrolly2" as worthy. This came to 14 layouts. In addition I keep around graphite and qwerty as reference layouts. So 16 layouts in total to compare.
2. My use of @ironcollar's excellent analyser [keycraft](https://github.com/rbscholtus/keycraft);
3. Dumping data from keycraft into Excel and applying @ec0's ranking bands for each metric (more about that in the section below, [Analysis - ways of speaking](#analysis---ways-of-speaking).)

4. Bringing to bear insights from KLD; and
5. Bringing to bear insights from AKL members in "Regard for inrolly2".

(4) and (5) have been useful to identify either:

* Patterns that aren't revealed in, or aren't obvious in, the keycraft or Excel output; and/or
* Patterns borne out by the experience of veterans in their use of layouts.

"My analysis" is ahead of trialling the winning layouts myself.

In "Regard for inrolly2" some mentioned the helpful [https://keyboard-layout-try-out.pages.dev/]( https://keyboard-layout-try-out.pages.dev/), as a quick way to do a software-based trial of layouts. Because you use qwerty to emulate how a different layout would feel. However, in my having learnt Graphite (even to a low WPM) my qwerty usage is somewhat borked. So I'm intending to trial the winning layouts - ints and wave2 - at the hardware level on my Voyager (which is easy to do with that keyboard). I have in mind I'll learn each layout to 20 wpm - ints first, then wave2 - and decide on the ultimate winner at that point.

Incidentally, that my qwerty usage is borked flags to me I may want to practice both a candidate/winning alt layout and qwerty at the same time. That is, to remain bi-layout competent. For I'll want to retain the ability to jump on qwerty for brief spouts of:

* Standard laptop usage (custom colstag keyboards and laptops are still a way off)
* Mobile phone (software) keyboards
* Gaming. Gaming layouts are probably necessarily stuck with qwerty as a reference. I don't think it would be practical to remap a game's keyboard commands to a non qwerty layout. I intend to retain a separate traditional qwerty rowstag keyboard for gaming. (I have and endorse a Keychron K1 Pro).

Anyway the point of my analysis has been to identify one or two layouts that will be worthy of trial.

## Analysis - ways of speaking

I'll demo keycraft commands as I use them on Windows and Powershell. Which should remain obvious on how to use on different platforms (keycraft itself is multiplatform).

If I reference a person with a "@" prefix, that will be their Discord user name.

I'll refer to a [keycraft metric](https://github.com/rbscholtus/keycraft?tab=readme-ov-file#supported-metrics) as defined in the linked readme, usually by using the acronym ("SFB", "3RL-IN", etc). @ironcollar has recently updated that readme (and added a few more metrics, and altered a few metric names) to be far clearer.

Note from keycraft > Supported Metrics (previously linked) "Bigram, skipgram, and trigram metrics follow the Keyboard Layouts Doc".

When I refer to metric **value** I'll either:

* If using ec0's 9 rung English word "Min, Very low, Low, Mid low, Mid, Mid high, High, Very high, Max" - I'll use that word. E.g. I might say "wave2-cs-ns has a very high FSB"; or
* Speak broadly to refer to the 3 rung band (within which there is the further division into three). To do this I'll use "Lowish", "Midish", or "Highish". E.g. I might say "wave2-cs-ns has a highish FSB".

## Analysis - keycraft customisation

### Layout customisation

After installing keycraft (v0.5.0) I copy and modify the 16 layouts of interest.

From example data\layouts\graphite.klf ...

```
# https://github.com/rdavison/graphite-layout
rowstag
~ b l d w z  ' f o u j ;
~ n r t s g  y h a e i ,
~ q x m c v  k p . - / ~
      ~ ~ ~  _ ~ ~
```

... is copied as data\layouts\graphite-cs-ns.klf ...

```
# https://github.com/rdavison/graphite-layout
colstag
~ b l d w z  ~ f o u j ~
~ n r t s g  y h a e i ~
~ q x m c v  k p ~ ~ ~ ~
      ~ ~ ~  _ ~ ~
```

That is, I've changed the "rowstag" keyword to "colstag". And I've blanked out the symbols with tildes ("~").

Evidently in keycraft both matter. E.g. `keycraft view graphite graphite-cs-ns` will produce differences in layout presentation and calculation (@ironcollar could say more).

<img src="KeycraftViewGraphiteGraphiteCSNS-2026-02-01-113443.png" alt="keycraft view graphite graphite-cs-ns" style="display:block; margin: 0 auto; width:80%;" />

### Weights file customisation

The keycraft `rank` command allows one to use a custom weights file. My weights file is on the right ...

<img src="DefaultVJohnWeightsFile2026-02-01-122234.png" alt="Default V John's Weights file" style="display:block; margin: 0 auto; width:80%;" />

In summary, compared to the default, I penalise higher ALTs and promote 2RL-IN and 3RL-INs.

My weights file differences are more shooting from the hip rather than being the result of some careful or deep meditation on the numbers. It's easy to change the rank order of layouts through small tweaks in the weights file. So the weights file is intended to produce a rank that situates us roughly; then from there look more closely at the metric scores for each layout. In other words I'm open to, as a notion before the start of analysis proper, disqualifying a layout that scores **better** than a layout I may keep.

### Corpus

keycraft comes with three corpora. I use the default, "shai", corpus.

@iSa tells us (in [AKL > Are there authoritative sources for the corpora: shai and akl?](https://discord.com/channels/807843650717483049/1467736504980869225/1467763160059482163))

> Shai: The default most analysers use, very large sample size corpus generated by cleaning the internet basically.

I assume that corpus is suitable, therefore, for optimizing for general English (essays, articles, etc).

## Analysis - the stats

So with keycraft installed, the following PowerShell ...

```powershell
Clear
Set-Location "C:\Program Files\Keycraft"
$LongList = @("flour-colstag-ns","flame-cs-ns","gallium-v2-cs-ns","graphite-cs-ns","heyyou-cs-ns",
    "hieamtsrn-cs-ns","inrolly2-cs-ns","ints-cs-ns","rain-cs-ns-cmini","seht-drai-cs-ns","sturde-cs-ns",
    "sturdy-cs-ns","stronk-cs-ns","trendy-cs-ns","wave2-cs-ns","qwerty-ns")
keycraft rank $LongList --weights-file john.txt --metrics extended --deltas graphite-cs-ns
```

... yields ...

<a href="keycraft-rank-16-layouts.png">
  <img
    src="keycraft-rank-16-layouts.png"
    alt="Keycraft rank 16 layouts"
    style="cursor: zoom-in;" />
</a>

