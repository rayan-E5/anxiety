# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: ایول!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *آه.* زدی تو خال.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: میدونی بچه؟...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: در واقع؛ زدی تو آمیگدالای چپ و راست من.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: تو من رو یاد جوونی خودم میندازی. وقتی داشتم از دست اون حیوون عذاب میکشیدم.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: خیلی خوشحالم که میتونم کمکت کنم اون هیولا رو مثل خودم بکشیش.

```
publish("act3",["roofhunter",2]);
```

r: هی! زودباش: جرات یا حق-

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: جرات!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: هاها! عالیه!

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: خب. اون استخر آبی کوچولو رو اون پایین می بینی؟

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: آره ... شش طبقه پایین تر؟

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: بپر توش.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: وایسا. چی؟

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: حیوون شروع کرده به ناله کردن. نه؟

```
publish("act3",["roofhunter",23]);
```

r: *وای نههه این خطرناکههه انجامش ندههه*

```
publish("act3",["roofhunter",22]);
```

r: بخاطر همین هیجان زیادی میخوایم! آرههه! خوش باش! دهنشو سرویس کن!

```
publish("act3",["roofhunter",10]);
```

r: به اون حیوون نشون بده به کتفمونم نیس!

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: ام.. ولی .. بعضی وقتا.. ترس یه دلیلی داره.

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: ودف؟ اون تبلیغات روانشناسی که میگن "احساس بد *خوب* است" رو باورت شده؟

```
publish("act3",["roofhunter",17]);
```

r: همون عوضی هایی که اینا رو اداره میکنن باعث افسردگی و اضطراب مان.

```
publish("act3",["roofhunter",18]);
```

r: سخنرانی های تد میگیرن تا بپذیریم بدبختیم و باید اون هیولای سادیست رو *در آغوش* بکشیم!!

```
publish("act3",["roofhunter",6]);
```

r: بچه؛ میدونم که میدونی اون حیوون چقدر امثال ما رو *آزار* میده. *شکنجه* میکنه.

```
publish("act3",["roofhunter",19]);
```

r: اون دوستمون نیست. یه وحشی هاره که باید رام بشه.

```
publish("act3",["roofhunter",20]);
```

r: یا یه گلوله تو کله اش فرو شه.

```
publish("act3",["roofhunter",27]);
```

r: وگرنه می بره.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: نه. اشتباه می کنی!

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: من نمی ذارم ببره!

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: آرههه! لعنتی. من بهت ایمان دارم بچه! بکشش!

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: نه نه نه نه نه نه

n: این بخش تو پایان ممکن دارد. یکی *خیلی خیلی* بد است.

b: نه نه نه نه نه نه نه نه نه نه نه

n: هوشمندانه انتخاب کن. از انسانت محافظت کن.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: قلدبهخذدلقذخهثدخحثقئخقحثنثقخح

`bb({ mouth:"normal" });`

n: موفق باشی

```
Game.clearText();
bb({ eyes:"start" });
```

[تو واقعا ممکنه اینجا بمیری انسان.](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[کارت احمقانه و خود ویرانگرانه ست.](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[این مریضا واقعا دوستت نیستن.](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: ت--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: ک--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: ا--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: میدونی؟ اگه قبلا میلیون ها بار امتحان نکرده بودی شاید باورت میکردم.

h: خودتو نخ نما کردی.

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: اونم امتحان کردی.

b: انسان، خواهش میکنم...

`hong({ eyes:"look_right" });`

h: اوه! متاسفم! یافته های پزشکی با روش خود درمانیم موافق نیستن؟

h: ببین کثافت: هرکی یه راهی داره تا تو رو خفه کنه.

`hong({ body:"look_up", eyes:"look_up" });`

h: بعضی آدما خودشون رو غرق کار میکنن.

`hong({ body:"look_down", eyes:"look_down" });`

h: بعضی غرق مواد مخدر، رابطه جنسی، فضای مجازی.

`hong({ body:"normal", eyes:"look_right" });`

h: بعضی خودشونو غرق بقیه میکنن.

`hong({ eyes:"angry" });`

h: من میخوام خودمو تو استخر اون پایین غرق کنم!

[تو مستی و این 6 طبقه ست.](#act3_bad_1_harm)

[بشکنه دستتی که نمک نداره. این تشکرته؟](#act3_bad_1_insult) `bb({eyes:"angry"});`

[خیلی خب. اعتراف میکنم. گند زدم.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: حتی اگه *توی آب* فرود بیای کشش سطحی دنده هات رو میشکنه و حداقل ضربه مغزی میشی.

h: عه
```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: یه بار یه پسر روس تو یوتیوب دیدم که این کارو کرد.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: ب.. ببخشید؟ *تشکر*؟!!

`bb({ eyes:"angry" });`

b: بله. من اصلا وجود دارم که از تو محافظت کنم.

b: کل زندگیم داشتم از مراقبت میکردم تا خش رو باسنت نیفته و حالا توی احمق داری...

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: هه!

`hong({ body:"laugh_2" })``

h: هاهاهاهاهاها!

`hong({ body:"laugh_3" })``

h: *هاهاهاهاهاهاهاها!*

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: وااااو این بزرگ ترین کشف کوفتی قرنه!

`hong({ body:"yell_2" });`

h: آره! تیکه گه گندیده خونی! گند زدی!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: نکته دیگه ای دارید جناب؟!

[ولی انتقام گرفتن راه حل نیست.](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[ولی این دفعه *واقعا* حق با منه.](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[من بهت آسیب زدم.](#act3_good_2a)


# act3_good_1_fail_revenge

b: باید با احساساتت رابطه سالم تری داشته باشی. نه اینکه غرقشون کنی توی-

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: پس لطفا؛ بطری رو بذار کنا و بیا-

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: لطفا... نکن...

h: نوار انرژیت وحشتناک خالیه آقا گرگه!

h: اگه جات بودم واژه های بعدیمو با دقت زیاد انتخاب میکردم!

`bb({ eyes:"normal" });`

[باشه. محافظت ازت رو تموم میکنم.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[من همیشه درست میگفتم.](#act3_bad_2_right)

[ببخشید.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: خب! برو بپر! واسم مهم نیست!

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: خیلی خب. بریم!

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: *نه وایسا وایسا وایسا نه این روانشناسی معکوسه تو باید برعکس چیزی که گفتم رو-*

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: داری خودتو نابود میکنی. به اصطلاح دوستات دارن ازت استفاده میکنن. تو داری از به اصطلاح دوستات استفاده میکنی.

`bb({ eyes:"sad" });`

b: پس لطفا! انسان!... تو من رو باور نداری؟

h: نه. تو هیچ وقت من رو باور نداشتی.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: بقیه گرگ های نگهبان انسان هایی دارن که *واقعا* برای آموزششون وقت میذارن.

b: بجای اینکه از گرگ های نگهبانشون بابت محافظت کردن متنفر باشن! چرا نمیتونی فقط-

`bb({ eyes:"normal" });`

h: پاسخ نادرست!

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"تنها چیزی که باید از آن ترسید ترس است."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *نترس! خوشحال باش!*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: هر آدم عاقلی میدونه احساسات منفی *بدن*.

`hong({ eyes:"less_angry" });`

h: خب! بخاطر همین بهشون میگیم منفی.

b: انسان... خواهش میکنم...

`hong({ eyes:"normal" });`

h: یه ذره پیش گفتم فقط میخوام از این همه درد رها بشم!

h: خب به آرزوم رسیدم! دیگه نه درد دارم، نه ترس و نه اضطراب.

h: کلا هیچی حس نمیکنم.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: من انقدر وسواس داشتم که هیچی بهت آسیب نرسونه که متوجه نشدم *خودم* دارم بهت آسیب میزنم...

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: نه! تف!

`hong({ body:"yell_1" });`

h: واقعا انقدر طول کشید تا بفهمی احمق؟!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: این همه مدت میتونستی ازم محافظت کنی! حالا فهمیدی احمق کونی؟

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: تو *متاسفی*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: برای چی *ببخشمت*؟

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[ببخشید که محافظ خوبی نبودم.](#act3_good_3_protector)

[ببخشید که بهت احترام نذاشتم.](#act3_good_3_respect)

[متاسفم.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[متاسفم که یه انسان افتضاح داشتم!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[متاسفم که بهت احترام نذاشتم.](#act3_good_3_respect)

[متاسفم که بهت آسیب زدم.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: وظیفه من این بود که خطر *واقعی* رو بهت گوشزد کنم. ولی من فقط واق واق میکردم!

`bb({eyes:"sorry_up"});`

b: برای هرچی واق واق میکردم. همیشه!

`bb({eyes:"sorry"});`

b: کاملا منطقیه که بخوای دهنمو گل بگیری.

`bb({eyes:"sorry_down"});`

b: متاسفم.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: من باید سگ نگهبان *تو* می بودم ولی طوری رفتار کردم انگار تو باید از *من* پیروی کنی.

`bb({eyes:"sorry_up"});`

b: محافظ با نگهبان زندان فرق داره. من مرز رو رد کردم.

`bb({eyes:"sorry_down"});`

b: متاسفم.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: من انقدر درگیر محافظت از *تو* بودم که نفهمیدم *من* دارم به تو آسیب می زنم.

`bb({eyes:"sorry_up"});`

b: من سگ بدی بودم.

`bb({eyes:"sorry_down"});`

b: متاسفم.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: آره. خب. به هر حال ایده احمقانه ای بود.

h: من این کارو کردم که بهمت بریزم. خب ریختم@

h: بیا این دور رو مساوی کنیم. اوکی؟

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: باشه.

h: خیلی خب.

n: *برابر*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: اوه! بیخیال! بعد از تمام بلاهایی که اون حیوون سرت آورد داری جا میزنی؟

r: مشکل چیه بچه؟ *ترسیدی*؟

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: آره.

h2: ترسیده ام.

`publish('hong-next')`

h2: و این اوکیه!

`publish('hong-next')`

h2: اوکیه که بترسی!

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: در رو قفل کرد؟!

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: no...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: نه نه نه

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: *نه!*

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
