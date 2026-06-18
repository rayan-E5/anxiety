# act1

```
SceneSetup.act1();
```

(...300)

n: و این اضطراب انسان است.

n: _تو_ اضطراب هستی

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: عه سلام! ما دوباره برگشتیم اینجا؟

`hong({eyes:"0_neutral"})`

n: وظیفه شما محافظت از انسانتان در برابر *خطر* است.

`bb({eyes:"look", mouth:"small_lock"})`

n: در واقع همین حالا انجام دوباره این بازی دارد برای او خطرآفرین می شود.

n: زود باش! درباره یک *خطر* به او هشدار بده

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: انسان! گوش کن. ما در خطریم. بازیکن...

[...می خواد دوباره شکنجه مون بده](#act1_replay_torture)

[...این بار یه راه حل جایگزین پیدا نخواهد کرد](#act1_replay_alternate)

[...دچار تضاد روایی خواهد شد](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: اون مجبورمون می کنه چنبره بزنیم و گریه کنیم.
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: اون مجبورمون می کنه گوشیت رو نابود کنیم چون دچار حمله عصبی شدی.
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: اون مجبورمون می کنه به میزبان مهمونی مشت *نزنیم*
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: کاری می کنه که به میزبان دلسوز ضد شرور مهمونی مشت بزنیم!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: خب حداقل این بار از پشت بوم نمی پریم پای...
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: اون مجبورمون می کنه از پشت بوم بپریم پایین.
{{/if}}

`bb({body:"fear"});`

b: همه این چیزهای وحشتناک برای ما اتفاق خواهند افتاد. و بعدش ما...

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: درسته. داستان در کل همونه ولی هر قسمت دو پایان اصلی داره. به علاوه کلی دیالوگ فرعی!

`bb({body:"fear"});`

b: بازیکن ناامید میشه، صفحه مرورگر رو می بنده، نرم افزار ما رو پاک می کنه و بعد ما...

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: یه ناهماهنگی چی؟

`bb({eyes:"normal"});`

b: داستان درباره این بود که چطور می تونید *انتخاب* کنید که با ترستون یه همکاری سالم بسازید.

`bb({eyes:"normal_right"});`

b: ولی تکرار بازی همون داستان رو نشون میده. که یعنی *انتخاب* تو اهمیتی نداره.

`bb({eyes:"narrow_eyebrow"});`

b: پس بین ساختار بازی و پیامش تناقض به وجود میاد.

`bb({eyes:"fear"});`

b: بنابراین خشت خشت این داستان روایی فرو می ریزه.

`bb({body:"fear"});`

b: و بعدش ما...

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: می میریییییییییییییییییییییییییییییم

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: خیلی خب. بیا به شخصیتمون برگردیم.

```
Game.clearText();
```

n4: (بگذار اضطرابت ور ور ور شبیه ترین چیز به ترس هات ور ور ور. خودت می دونی.)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: خیلی خب. گرگم برگشته. عااااااااااالیه.

`hong({eyes:"0_neutral"})`

n: وظیفه شما حفاظت از انسانتان در برابر *خطر* است.

`bb({eyes:"look", mouth:"small_lock"})`

n: در واقع همین الان آن ساندویچ دارد او را در خطر قرار می دهد.

n: زود باش! بهش هشدار بده.

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: گوش کن انسان! ما در خطریم. خطر...

`bb({body:"squeeze"})`

n4: (به اضطرابت اجازه بده بیاد و بازی کنه. شبیه ترین گزینه به ترس های _خودت_ رو انتخاب کن)

(#act1_normal_choice)

# act1_normal_choice

[ما داریم تنهایی ناهار می خوریم. دوباره!](#act1a_alone) `bb({body:"squeeze_talk"})`

[ما موقع غذا خوردن بازدهی نداریم!](#act1a_productive) `bb({body:"squeeze_talk"})`

[اون نون سفید برامون بده!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: نمی دونستی تنهایی به اندازه کشیدن 15 نخ سیگار در روز باعث مرگ زودرس میشه؟

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (منبع: Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: اممم... ممنون بابت ذکر منبع ولی...

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: که یعنی اگر همین الان نریم پیش یه نفر ما...

`bb({body:"panic"})`

b: می میرییییییییییییییییییییییییییییییم

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: تو *ترس از طرد* رو استفاده کردی.

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: همین الان لپ تاپت رو در بیار و یه ذره کار کن.

`hong({eyes:"0_annoyed"})`

h: اممممم... ترجیح میدم خرده نون نره توی صفحه کلیـ...

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: اگر به جامعه سود نرسونیم انگل اجتماعی هستیم!

b: جامعه می ره پیش جامعه پزشک تا بهش داروی ضد انگل بده و ما...

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: می میریییییییییییییییییییییم

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: تو *ترس از آدم بدی بودن* رو استفاده کردی

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: اون مطالعات تایید شـ...

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: گندم فراوری شده باعث میشه قند خون بگیریم و بعد باید تمام اندام هامون رو قطع کنیم و بعد ما...

`bb({body:"panic"})`

b: می میرییییییییییییییییییییییییم
```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: تو *ترس از آسیب دیدن* رو استفاده کردی.

(#act1b)

# act1b

n: اون فوق العاده موثره.

`bb({mouth:"smile", eyes:"smile"});`

b: می بینی انسان؟ من سگ محافظ وفادارتم!

`bb({body:"pride_talk"});`

b: به غریزه ات اعتماد کن. احساسات تو همیشه معتبرند.


`bb({body:"pride"});`

n: نوار انرژی انسان خود را به 0 برسانید.

n: برای محافظت از نیازهای جسمی + بدنی+ اخلاقی آنها می توانید از این موارد استفاده کنید:

n: ترس از *آسیب دیدن* #harm#

n: تر از *طرد* #alone#

n: و ترس از *آدم بدی بودن* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (نکته: گزینه هایی را انتخاب کنید که شخصا عمیق ترین و تاریک ترین ترس های شما هستند!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: می دونی؟ احتمالا بهتره الان گوشیمو چک کنم.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: از انسان خود محافظت کنید.

n: در برابر دنیا، در برابر مردم، در برابر خودش.

n: موفق باشی.

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: دور نخست: *مبارزه!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: عه! فید فیسبوک گفته این آخر هفته یه مهمونی برگزار میشه.

`bb({eyes:"uncertain"});`

b: مگه اون یاروی عجیب غریف *هر* آخرهفته مهمونی نمی گیره؟

`bb({eyes:"uncertain_right"});`

b: دارن تلاش می کنن چه خلأ ردونی ای رو پر کنن؟ باید از درون خیلی آشفته باشن.

`hong({eyes:"surprise"});`

h: منم دعوت شده ام؟

`bb({eyes:"fear", mouth:"normal"});`

b: خب پس

[بگو آره وگرنه از تنهایی می میریم!](#act1c_loner)

[بگو نه. اونجا پر از مخدرهای سمیه!](#act1c_drugs)

[نادیده اش بگیر. ما فقط مهمونی ها رو افسرده می کنیم.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: روزی 15 نخ سیگار انسان! پانزده نخ!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: اون وقت هیچکس برای خاکسپاریمون نمیاد. خاکسترمون رو می ریزن تو دریا و نهنگ ها می خورنمون.
{{/if}}

{{if !_.fifteencigs}}
b: و ما به مدفوع نهنگ تبدیل میشیم.
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: خب آره. ما باید به اون مهمونی بریم.
{{/if}}

{{if _.parasite}}
b: فقط لپ تاپ رو بیار تا بتونیم کار کنیم و انگل جامعه نباشیم.
{{/if}}

{{if _.whitebread}}
b: فقط تا وقتی نون سفید نخورن!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: خدایا! اگه خفه میشی باشه.

h: میگم آره.

{{if _.whalepoop}}
b: مدفوع نهنگ انسان! مدفوع نهنگ!!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: یا حتی بدتر ... نون سفید!
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: انقدر نون سفید و شیشه مصرف خواهیم کرد که دیگه جسدمون توی کوره آدم سوزی جا نشه.
{{/if}}

{{if !_.whitebread}}
b: .انقدر اوردوز خواهیم کرد که مرده شور با دیدن جسدمون تعجب میکنه
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: بگذریم. نمی تونیم بریم مهمونی. اگه کار نکنیم انگل اجتماعی میشیم.
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: خدایا. اگه خفه میشی باشه.

h: میگم نه.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: تنها کاری که همیشه می کنیم اینه که یه گوشه میشینیم و درباره اینکه تنهایی به اندازه 15 نخ سیگار در روز کشنده ست گریه میکنیم.
{{/if}}

{{if _.parasite}}
b: تنها کاری که همیشه تو مهونی میکنیم نگرانی درباره اینه که چطور مفید باشیم.
{{/if}}

{{if _.whitebread}}
b: تنها کاری که همیشه می کنیم ترسیدن درباره اینه که چطور غذاهای ناسالم ما رو خواهند کشت.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: خدایا من تعجب می کنم چرا!

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: پس اگر بریم، حالشون رو بد می کنیم. و اگر دعوتشون رو رد کنیم، باز هم حالشون رو بد می کنیم.

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: تنها کاری که ما می کنیم بد کردن حال مردمه. پس حال خودمون هم باید بد باشه.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: آه. اگه خفه میشی باشه.

h: دعوت رو نادیده می گیرم.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: هعی. فیسبوک خیلی شلوغه. من یه چیز آروم تر میخوام که کمتر اضطراب آور باشه!

`hong({eyes:"neutral"});`

h: توییتر چه خبره؟

`bb({eyes:"look"});`

[وای نه! اون خبر وحشتناک رو نکاه کن!](#act1d_news)

[وای نه! اون یه توییت مخفیانه درباره *ما*ست؟](#act1d_subtweet)

[عه! یه گیف از یه گربه که داره شیر می خوره!](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: خدای من! انگار دنیا داره نابود میشه! نه؟

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: همه چیز دارد پایان می یابد. همه چیز دارد می میرد. ما همه محکوم به فنا هستیم و هیچ کاری از دستمون بر نمیاد.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: بیا این داستان رو ریتوییت کنیم.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: باشه. ریتوییتش می کنم. فقط لطفا دهنت رو ببند.

`hong({mouth:"neutral", eyes:"annoyed"});`

h: ولش کن. بیا یه نگاه به اسنپ چت بندازیم!

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: این یه توییت کاملا زیرپوستیه. من مطمئنم

`hong({eyes:"annoyed"});`

h: فکر نکنما!

`bb({eyes:"narrow", mouth:"small"});`

b: ولی اگر همه شون در حال حرف زدن پشت سر ما باشن چی؟

h: اونا این کارو نمیـ

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: جلوی پشت سرمون!

`hong({eyes:"sad", mouth:"sad"});`

h: من فــ

`bb({eyes:"narrow", mouth:"small"});`

b: ولی *اگر باشه*

h: خـ

`bb({eyes:"narrow_eyebrow"});`

b: *اگر باشه*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: خ..خیلی خب... اسنپ چت رو امتحان می کنم.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: آره! چه بامزه! ریتوییتش کردم. من ا...

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: گربه ها نمی تونن شیر رو هضم کنن و ما آدم های وحشتناکی هستیم که از آزار حیوانات لذت می بریم.

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: خ...خیلی خب. اسنپ چت رو امتحان می کنم.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: هعی. عکس های دیشب! پس مهمونی های هفتگی *این* شکلین.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: هوف. برای اضطراب من زیادی شلوغ بنظر میرسه.

h: شاید نباید دعوت رو می پذیرفتم؟

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[مثل یه احنق جوابمون رو عوض کنیم؟!](#act1e_yes_dontchange)

[جوابتو عوض کن. خیلییی شلوغه!](#act1e_yes_changetono)

{{if _.subtweet}}
[آره! اونا داشتن پشت سرمون حرف میزدن!](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[وایسا. ما بدون بررسی درستیش ریتوییت کردیم](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[میدونی؟ فرم بدنت خیلی بده.](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: اونا روی ما حساب کرده بودن که بریم و ما داریم بهشون خیات می کنیم؟ می خوای تنها بمیری؟

{{if _.fifteencigs}}
b: پانزده. سیگار.
{{/if}}

{{if _.whalepoop}}
b: مدفوع. نهنگ.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: خفه شو! خفه شوو! همینطور نگهش می دارم.

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: تا حالا درباره رم کردن مردم نشنیدی؟

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: در سال 2003 یه کلوپ شبانه توی رود آیلند آتش گرفت و وحشت مردم باعث شد درهای خروجی رو ببندن. اون شب 100 نفر سوختن و مردن!

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: می خوای این برای ما اتفاق بیفته؟

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: بگو نه بگو نه بگو نه بگو نه بگو نه بگو نه بگو ن-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: خفه شو! خفه شوو! می گم نه. خدایا!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: عامم.. خیلی جالب بنظر می رسه!

h: شاید نباید دعوت رو رد می کردم؟

`bb({mouth:"normal", eyes:"normal"});`

[جوابمون رو عوض کنیم؟ مثل یه احمق؟](#act1e_no_dontchange)

[جوابمون رو عوض کن. نباید تنها بمیریم!](#act1e_no_changetoyes)

{{if _.subtweet}}
[اونا کاملا داشتن پشت سرمون حرف میزدن](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[صبر کن. ما بدون بررسی درستی ریتوییتش کردیم.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[میدونی؟ فرم بدنت واقعا بده.](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: همه داشتن روی ما حساب می کردن!

b: که ولشون کنیم و بذاریم یه مهمونی خوب بدون چیزهای وحشتناک حال بهم زن داشته باشن. {{if _.whitebread}}white-bread-munching{{/if}} مثل تو..


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: خفه شو! خفه شوو! جوالم رو منفی نگه می دارم.

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: تنهایی مزمن سطح کورتیزول و خطر ابتلا به بیماری های قلبی عروقی و سکته قلبی را افزایش می دهد.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: پانزده. سیگار.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: خفه شو. خفه شوو! میگم آره. خدایا!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: تمام توییت های مشکل دارمون دوباره راه افتادن.

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: قراره مچمون رو بگیرن، طردمون کنن و ما رو سوژه ی کل اینترنت کنن.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: چرا تو اینجوری ای؟!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ما داریم مطالب نادرست پخش می کنیم. ما داریم به اعتماد به رسانه های آزاد ضربه می زنیم.

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ما دلیل بروز فاشیسم از ویرانه های دموکراسی هستیم.

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: چرا ما اینجوری ایم؟

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: می خوای ستون فقراتت هم عین عقلت تاب برداره؟ انقدر روی صفحه گوشت خم نشو.

```
bb({body:"meta"});
```

b: این یعنی تو هم.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: چرا تو اینجوری ای؟

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: اممم... خیلی جالب بنظر می رسه!

h: شاید نباید اون دعوت رو نادیده می گرفتم؟

`bb({mouth:"normal", eyes:"normal"});`

[به نادیده گرفتن ادامه بده. ما هنوزم به مهمونیا گند میزنیم.](#act1e_ignore_continue)

[راستش؛ بگو آره.](#act1e_ignore_changetoyes)

[راستش؛ بگو نه.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: فکر میکنم یه جورایی بی ادبانه ست که به محل نذاشتن ادامه بدم. نه؟

`bb({eyes:"normal_right"});`

b: خب بقیه هم همیشه *ما* رو نادیده می گیرن.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: پس بیا فقط مقابله به مثل کنیم.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: تو... داری می ذاری خوش بگذرونم؟

b: خب منظورم این بود که تنهایی *می تونه* ما رو بکشه.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: خیلی شلوغه. شلوغی خطرناکه.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: هرچی. یه نوتیف جدید از تیندر!

`bb({eyes:"uncertain"})`

b: چی؟ اون نرم افزار دوست یابی؟!

`hong({eyes:"annoyed"})`

h: این یه نرم افزار دوست یابی نیست! فقط یه راه برای ملاقات با آدم های جدیـ..

`bb({eyes:"narrow"})`

b: این یه نرم افزار دوست یابیه.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: اوو! یه نفر پیدا کردم! گوگولی بنظر میرسه:)

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: لطفا این یکی رو خراب نـ..

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: خطر خطر خطر خطر خطر خطر خطر خطر خطر خطر
`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[ما داریم توسط دیگران *مصرف* می شویم.](#act1f_used_by_others)

[ما داریم دیگران را *مصرف* می کنیم.](#act1f_using_others)

[اون یه قاتل سریالیه.](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: رابطه های یهویی شاید بتونن خالی بودن اون پایین رو پر کنن.

b: ولی هیچ وقت نمی تون خلا ها رو پر کنن...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *اینجا*

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: نکته اینه که ما قراره تنها بمیریم.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: فکر کردی ملت کارت بازین که باید همه شون رو دور خودت جمع کنی؟

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: آهنگ پوکمون...

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: من میخوام هرزه ترین باشم..

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ طوری که هیچکس هیچوقت نبوده 

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ بدن های جذاب

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ اعضای عرق کرده

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ پری-مون . من باید برم..

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: نکته اینه که ما موجودات حیله گری هستیم.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: اون تو یه چاه گیرت می مدازه و بهت نون سفید میده تا چاق بشی و بتونه از پوستت به عنوان چرم استفاده کنه.
{{/if}}

{{if _.parasite}}
b: با یه دفتر برنامه ریزی کتکت میزنن و بهت میگن باید بازدهی می داشتی احمق.
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: اونا گوشتت رو تکه تکه میکنن و از روده هات که عین ریس به سقف بستن آویزون می کنن و خونت رو توی پیاله سر می کشن.
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: این برای یه دعوت مهمونی چطوره؟
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: خیلی از این بازی خسته ام.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"تنهایی ما رو خواهد کشت."... {{/if}}
{{if _.parasite}}"ما انگل جامعه ایم."... {{/if}}
{{if _.whitebread}}"اونو نخور. ما رو می کشه."... {{/if}}
{{if _.subtweet}}"دارن مستقیم پشت سرمون حرف می زنن."... {{/if}}
{{if _.badnews}}"دنیا داره منفجر میشه."... {{/if}}
{{if _.hookuphole}}"ما تنها خواهیم مرد."... {{/if}}
{{if _.serialkiller}}"اون یه قاتل سریالیه."... {{/if}}
{{if _.catmilk}}"گربه ها نمی تونن شیر رو هضم کنن."... {{/if}}
{{if _.pokemon}}یه آهنگ تقلیدی چرند... {{/if}}

h: من فقط میخوام زندگیم رو بکنم.

h: من فقط میخوام ... از تمام این درد رها بشم.

`bb({eyes:"look_sad"});`

b: هی... انسان...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: درست میشه.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: به عنوان گرگ نگهبان وفادارت همیشه مراقب خطر هستم و ازت نگهداری می کنم.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: قول میدم.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: آخرین اپ: اینستاگرام. چیا گذاشتن؟

`hong({eyes:"sad"});`

h: این... عکس های بیشتر از مهمونیه.

`hong({mouth:"sad"});`

h: همه خیلی خوشحال بنظر میرسن. آزاد از ترس و اضطراب.

`hong({mouth:"anger"});`

h: خدایا چرا من نمیتونم مثل اونا باشم؟ چرا نمیتونم *عادی* باشم؟

`bb({eyes:"normal_right"});`

b: حالا که درباره مهمونی آخرین هفته صحبت میکنی... تصمیم نهایی من اینه:

`bb({eyes:"normal"});`

[باید بریم.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[نباید بریم.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: ما نبـ..

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: خفه شو.

`hong({body:"2_you"});`

h: تو

(...500)

b: چ

(...1500)

`bb({eyes:"wat_2"});`

b: چی؟

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: میرم که جواب مثبت بدم.

{{if _.act1g=="go"}}
h: نه چون تو میخوای بدم. چون *خودم* میخوام.
{{/if}}

{{if _.act1g=="dont"}}
h: دقیقا چون *تو* نمیخوای.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: تو من رو کنترل نمی کنی.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: حالا ببخشید که یه گاز لعنتی به این ساندویچ میزنم.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[آه تو می میری.](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[آه همه از ما بدشون خواهد اومد.](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[آه ما آدم های ترسناکی هستیم.](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: وای ما می میریم. وااااااااااای

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: وای همه از ما متنفر میشن. واااااااای

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: وای ما آدم های وحشتناکی هستیم. وااااااااای.

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: تبریک!

(...500)

n: شما در محافظت از نیازهای بدنی + اجتماعی + اخلاقی انسانتان پیروز شدید!

n: نگاه کنید او چقدر سپاس گزار است!

(...500)

n: حالا که انرژی او به صفر رسیده شما می توانید مستقیما رفتار او را کنترل کنید.

`bb({mouth:"smile", eyes:"normal"});`

n: حرکت آخرت را انتخاب کن.

`bb({mouth:"small_lock", eyes:"fear"});`

n: *به او پایان بده*

[{FIGHT: گوشی اضطراب آورت را تنبیه کن!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FLIGHT: چنبره بزن و گریه کن!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: گوشیت باعث شد دچار حمله عصبی بشی!

`bb({eyes:"anger"})`

b: زاکربرگ و شریکاش دارن سلامت روان تو رو برای سرمایه خودشون می دزدن!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: گوشیت رو تنبیه کن! نابودش کن! بکشش!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: -بکشش بکشش بکشش بکشش بکشش بکشش بکشش بکشش بکشش بکشش بکشش بکشش بک

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: سراسر دنیا پر از خطره.

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: همون کاری رو بکن که آرمادیلو میکنه. برای دفاع از خودت مثل یه توپ دور خودت حلقه بزن.

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: چنبره بزن و گریه کن چنبره بزن و گریه کن چنبره بزن و گریه کن چنبره بزن و گریه کن چنبره ب-

(#act1j)

# act1j

`SceneSetup.act1_outro()`
