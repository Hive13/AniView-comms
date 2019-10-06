# AniView-comms

An attempt at interfacing with the [AniView 3000-1](http://www.lumenchina.com/page-164-146-j0xril.html) display that Hive13
acquired.

So far, this repository is just a dump of notes and photos I've been taking.

As the daughterboard has the identifier `DS06ADC_KB04 VER.A` on it, I
am guessing it is the KB04 referred to in that link, which gives this
pinout:

```
 -------------------------
|  A  B  C CK LD  R  G  D |
| OE  N  N  N  N  N  N  N |
 -------------------------
```

The "plug board CAM" link is down, but [Wayback Machine remembers](https://web.archive.org/web/20161224033255/http://www.lumenchina.com/page-164-146-j0xril.html): [KB04.rar](https://web.archive.org/web/20161224033255/http://www.2008led.com/front/action/file/downloadAction.do?id=4324).

## Original wiring

This originally had the bottom board's "Input" port connected to a WeMo D1 mini.

Looking at the "Input" port on the board (yes, I made up this numbering myself):

```
 -------------------------
|  1  3  5  7  9 11 13 15 |
|  2  4  6  8 10 12 14 16 |
 -----------    ----------
```

Input pins connect to WeMo D1 mini pins like this:
 - 1 - D1
 - 2 - D2
 - 3 - D0
 - 4 - G
 - 5 - D4
 - 7 - D3
 - 11 - D6
 - 15 - D5

## Photos

![back](photos/back.jpg)

![daughterboard](photos/daughterboard.jpg)

![mainboard](photos/mainboard.jpg)
