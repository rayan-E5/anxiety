# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[بازی کن!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: قبل از اینکه شروع کنیم؛ چطور دوست داری بخونی؟

`publish("show_options_bottom")`

# intro-start-2

n3: حالا بیاید داستانمون رو شروع کنیم ...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: این انسان است.

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: و این اضطراب انسان است.

n: _تو_ اظطراب هستی

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: نه نه نه. گوش نمی دم. می رم گوشیم رو چک کنم.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: وظیفه شما محافظت از انسانتان در برابر خطر است.

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: هوف! دوباره داری زندگیت رو توی توییتر تباه می کنی؟

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: آره خیلی تعجب آوره که چرا بیشتر وقت ها نمی شینم به افکارم گوش کنم.

`hong({eyes:"neutral"});`

n: سریع باش! درباره یک *خطر* به او هشدار بده.

```
bb({eyes:"look"});
```

[وای نه. اون خبر وحشتناک رو ببین!](#act1d_news)

[وای نه. اون یه توییت مخفیانه درباره *ما*ست؟](#act1d_subtweet)

[اوه! یه گیف از یه گربه که داره شیر می خوره.](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: عه آره. بامزه ست! مـ

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: گربه ها نمی تونن شیر رو هضم کنن. ما آدم های وحشتناکی هستیم که از آزار حیوانات لذت می بریم.

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



