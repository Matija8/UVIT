
# УВИТ Увод у рачунарске мреже

## Улога и начин рада рачунарских мрежа

Коришћење рачунарских мрежа:

- У данашње време скоро незамисливо коришћење рачунара који нису повезани са другим рачунарима

- Рачунари су стављени у нове улоге, број корисника све већи

- У мреже се повезују и паметни телефони, таблети, али и телевизори, кућни уређжаји, сензори итд.

- Обједињавање телекомуникационих услуга: јединствена мрежна инфраструктура за пренос гласа, података, радио и ТВ сигнала

- Интернет ствари (internet-of-things, IoT) предвиђжа умрежавање свих свакодневних објеката који нас окружују

Улога рачунарских мрежа:

- Комуникација: електронска пошта, друштвене мреже, Скајп (Skype), Вибер (Viber),...

- Дељење информација и података: распоред часова, ред вожње итд.

- Дељење софтвера: куповина карте преко веба, одређивање руте путовања, реализација банкарске трансакције итд.

- Дељење хардверских ресурса: штампача, скенера итд.

![пример рачунарске мреже](assets/images/network-example01.jpg)

Најчешћи начини извршавања послова у рачунарским мрежама су:

- Клијент-сервер окружење: коришћење веба, електронске поште

  - сервер пружа своје ресурсе (веб сервери, сервери БП, прокси сервери...)

  - клијент иницира контакт ради коришћења тих ресурса

- Мрежа равноправних рачунара (peer-to-peer, P2P): BitTorrent

![клијент-сервер и мрежа равноправних рачуара](assets/images/klijent-server-peer-to-peer.png)

## Компоненте рачунарских мрежа

Рачунарска мрежа је систем који се састоји од скупа **хардверских уређаја** медусобно повезаних **комуникационом опремом** и
снабедевених одговарајућим **контролним софтвером**, којим се остварује контрола функционисања система тако да је омогућен пренос
података измеду повезаних уређаја.

Дакле, компоненте мреже су:

- Мрежни хардвер

- Комуникациони канали

- Мрежни софтвер

### Мрежни хардвер

Да би уређај могао бити умрежен неопходно је да садржи специјализован део хардвера намењен умрежавању, који се
сматра делом комуникационе опреме.

Обично је то мрежна картица (мрежни адаптер или ЛАН картица – network interface controller, NIC), која се уграђује у рачунар и
омогућава уређају физички приступ мрежи.

![мрежни адаптер](assets/images/network-card.png)

Карактеристике:

- Излаз из мрежне картице је најчешће RS45 прикључак на који се прикључује тзв. UTP кабл.

![UTP aадаптер](assets/images/UTP-cable-plugin.png)

- Скоро сви десктоп рачунари имају уграђжену NIC картицу, док преносни имају уграђжену картицу за бежично повезивање (WNIC)

![WNIC aадаптер](assets/images/WNIC-card.png)

- Сваку мрежну картицу карактерише јединствена физичка (MAC) адреса којом се уредај јединствено идентификује приликом
комуникације

- Осим мрежних картица, за умрежавање се користе **модеми** (телефонски, кабловски), као и други слични уредаји

Модем (модулатор-демодулатор) је урежђај који конвертује дигитални сигнал у аналогни који се преноси, а затим обрнуто конвертује
пренети сигнал у дигитални; користи се за кабловски или АДСЛ приступ интернету

Модем се обично закупљује од добављача интернета и прикључује на парице фиксне телефоније, коаксијалне каблове кабловске телевизије или 
бежичне мреже мобилних оператера

![АДСЛ модем са бежичним рутером](assets/images/ADSL-modem.png) ![кабловски модем](assets/images/cable-modem.png))

Хаб, мост, свич и рутер – мрежни хардвер који служи за прослеђивање
комуникације између рачунара у мрежи режа и повезивању мреже
са Интернетом

```
Хаб, свич и рутер
```

Један уређај може обављати висе задатака: нпр. уређај за
успостављање бежичне комуникације има улогу приступне тачке,
свича и рутера (омогућава даљу везу са Интернетом)

```
Пример уређаја који представља приступну тачку, свич и рутер
```

### Комуникациони канали

л Комуникациони канали су каблови или бежични медијуми који преносе
податке електромагнетним таласима (радио-таласима, оптичким
таласима, микроталасима и сл.)

л Основна мера квалитета комуникационог канала јесте брзина
преноса или проток (тхроугхпут, бандwидтх) која се мери бројем
битова који се могу пренети у једној секунди (бит/с)
¡Узимајући у обзир актуелне технологије преноса на рачунарским
мрежама, чешће се користи јединица Мегабит у секунди Мбпс,
или Гигабит у секунди Гбпс

л Друга важна мера квалитета је кашњење (латенцy) - време
потребно да се компонента припреми за приступ подацима (мери
се у микросекундама у локалним мрежама и милисекундама у
оквиру већих мреза)


л Брзина преноса је физичка карактеристика комуникационог канала и
зависи од фреквенцијског опсега који се може пропустити кроз канал
без губитка сигнала

л С обзиром да је брзина преноса података сразмерна
фреквенцијском опсегу, са слике се јасно види због чега оптички
каблови дају најбоље перформансе

```
Подела електромагнтног спектра
```

#### Ожичене комуникације

```
о Укрштене парице - најкоришћенији начин комуникације
лУређаји се повезују коришћењем увијених упарених изолованих бакарних
жица, слично повезивању обичних телефона
лЖице се упарују и увијају како би се смањиле сметње у комуникацији
лУТП каблови (унсхиелдед тwистед паир) категорије 3 користе се у фиксној
телефонији, а категорије 5 или 6 у локалним мрежама; проток око 100 Мбпс
(брзи Етхернет), па и 1 Гбпс (гигабитни Ехтернет)
```
```
Схематски приказ укрштене парице
```
```
Изглед укрштене парице
```


```
¡Коаксијални каблови - обично се користе за телевизијске кабловске
системе, а користе се и у ЛАН мрежама итд.
лКаблови се састоје од централне бакарне или алуминијумске жице обмотане
савитљивим изолаторским слојем, око којега је опет обмотан проводни слој
танких жица, све обмотано спољашњом изолацијом
лКоаксијални каблови омогућују брзину преноса до 200Мбпс (чак и до
500Мбпс), уз мању осетљивост на електромагнетне сметње
```
```
Схематски приказ коаксијалног кабла
Изглед коаксијалног кабла и конектора
```

```
¡Оптички каблови - праве се од великог броја (стотина, хиљада) веома
танких стаклених влакана умотаних у заштитни слој
лПодаци се преносе светлосним таласима које емитује мали ласерски уређај
лНа овакве каблове не утичу сметње проузроковане електромагнетним
зрачењима
лСкупи су и компликовани за инсталацију, па се углавном користе за
осовински део мреже (мрежну кичму), на који се онда коаксијалним
кабловима или укрштеним парицама повезују појединачни уређаји
лНајчешће се користе за брзе мреже,
које имају брзину од 10 Гбпс навише
```
```
Схематски приказ оптичког кабла
Изглед оптичког кабла
```

#### Бежичне технологије

```
¡Не користе каблове за пренос података
¡То је посебно практично у случају преносивих рачунара, мобилних
уређаја или релативно удаљених локација за које би успостављање
кабловске мреже било недопустиво скупо
¡Уместо каблова користе се радио таласи, микро таласи, инфрацрвени зраци
¡Подаци се преносе модулирањем амплитуде, фреквенције или фазе таласа
¡Најчешће се користе следеће бежичне технологије:
лБлуетоотх – користи се за комуникацију на веома малим раздаљинама
(до десет или до сто метара у зависности од класе уредаја)
Брзине преноса иду до 3Мбпс
Користи радио таласе, може да проде и кроз чврсте препреке
Користи се углавном за комуникацију рачунара са периферијским уредајима
као и у мобилној телефонији.
```

```
¡Најчешће се користе следеће бежичне технологије :
лБежични ЛАН - (WЛАН, WиФи) технологија која користи радио таласе за
бежичну комуникацију више уређаја на ограниченом растојању (неколико
десетина или стотина метара)
У зависности од стандарда, брзина преноса иде од 10Мбпс до 50Мбпс (у
најновије време и до 600Мбпс)
Најраширенији стандард за бежичну ЛАН комуникацију је ИЕЕЕ 802.
Мрежи се приступа преко приступних тачака (аццесс поинт)
Област простора у којој је мрежа доступна назива се врућа тачка (хот
спот)
лБежичне градске мреже (WиМАX) покривају шира подручја и дају проток до
40 Мбпс
лЋелијски системи - начин преноса података веома сличан оном који се
користи у мобилној телефонији
За комуникацију се користе радио таласи и системи антена које покривају
одредену географску област, при чему се сигнал од одредишта до циља
преноси преко низа антена
```

Математички факултет (^) владаф@матф.бг.ац.владаф@матф.бг.ац.рс рс 20 / 53

лЗемаљски микроталаси - користе антенску мрежу на Земљи
За комуникацију користе микроталаси ниске фреквенције који захтевају да
антене буду оптички видљиве, тако да се оне обично смештају на високе
тачке (врхове брда, торњеве, небодере)
Антене могу да буду удаљене и до педесетак километара
лКомуникациони сателити – користе микроталасе за комуникацију тако што се
пренос између две тачке које немају оптичку видљивост остварује
попречном комуникацијом преко комуникационих сателита
Сателити се обично налазе у орбити на висини од 36 хиљада километара
На овај начин се, поред рачунарске комуникације, обично преносе
телевизијски и телефонски сигнал
Брзина комуникације је релативно мала (нпр. 100Мпс) у поредењу са
оптичким кабловима, али ипак има неколико сценарија у којима је коришћење
сателитске комуникације погодније

### Мрежни софтвер

л Неопходан је за функционисање рачунарских мрежа

л Да би се савладала комплексност рачунарских мрежа, мрежни
софтвер се организује хијерархијски

л Мрежни софтвер обухвата разне слојеве: од системског софтвера
ниског нивоа до апликативног софтвера

л Слојевитост олакшава програмирање мрежног софтвера - аутори
апликативног софтвера не морају да брину о детаљима мрежне
комуникације
¡На пример, програмер прегледача веба не треба да мисли о томе да ли
ће веб странице примати преко бежичне мреже или преко Етхернет мреже
лОн треба да се концентрише само на аспекте значајне за његову
конкретну апликацију
лСве ниже детаље мрежне комуникације он треба да препусти нижем слоју
мрежног софтвера (који је присутнан у оквиру оперативног система, или чак
самог мрежног хардвера)


л Најгрубље посматрано, мрежни софтвер може да се подели на два
нивоа:

1. Мрежни софтвер који омогућује коришћење различитих мрежних уредаја,
    нпр. мрежних картица или модема, јесте мрежни софтвер ниског нивоа
    Ова врста софтвера налази се обично у језгру оперативног система,
    углавном у облику управљача периферним уредајима, тзв. драјвера
    Драјвер управља рачунарским хардвером и комуникационом
    опремом
    Корисник никада не користи овај софтвер директно, у општем случају он
    није ни свестан да тај софтвер постоји
2. Основни задатак мрежног софтвера високог нивоа је да пружи услуге
    мрежним апликацијама које корисници користе
    Ове апликације пружају различите услуге корисницима на мрежи, као што
    је слање и пријем електронске поште, прегледање веба и сл.

л Данас оперативни системи садрже све нивое мрежног софтвера,
осим апликативног

## Захвалница

Делови материјала ове презентације су преузети из:

- Скрипте из предмета Увод у веб и интернет технологије, на
Математичком факултету Унивезитета у Београду, аутор проф. др
Филип Марић

- Презентација из предмета Увод у веб и интернет технологије, на
Математичком факултету Унивезитета у Београду, аутор др
Весна Маринковић

- Скрипте из предмета Информатика на Универзитету Милано Бикока,
аутор др Дарио Пешини