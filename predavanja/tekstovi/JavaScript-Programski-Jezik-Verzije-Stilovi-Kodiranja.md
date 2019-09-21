
# УВИТ - Програмски језик ЈаваСкрипт

[Владимир Филиповић](https://vladofilipovic.github.io/index-cy.html){:target="_blank"}

## Верзије језика ЈаваСкрипт

### Актуелна ECMAScript верзија

### Динамика појаве нових верзија

### Шта је то TC39

## Стилови кŏдирања

Стил кŏдирања за ЈаваСкрипт у ствари представља скуп конвенција које се користе при писању ЈаваСкрипт програма.

Стил кŏдирања се обично описује као споразум који склапају чланови програмерског тима, како би одржали конзистентност програмског кŏда у пројекту.

Чак и ако је тим једночлан, опет се стил кŏдирања може посматрати као споразум који програмер склапа сам са собом, како би програмски кŏд био у складу са сопственим програмеровим стандардима.

Постојање фиксних правила за форматирање програмског кŏда умногоме помаже да кŏд буде читљивији и лакши за одржавање.

### Популарни стилови кŏдирања

Поред многобројних постојећих, у овом тренутку су најпопуларнији стилови кŏдирања описани са следећа два документа:

- [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html){:target="_blank"}

- [AirBnb JavaScript Style Guide](https://github.com/airbnb/javascript){:target="_blank"}

Уколико радите на тимском пројекту, добра је пракса да се стил кŏдирања усагласи на почетку и да се усаглашени документ постави тако да у сваком тренутку  буде доступан свим члановима тима.

### Конвенције кŏдирања које су коришћене у оквиру овог курса

- У примерима и у опису конструкција биће коришћена актуелна верзија ЈаваСкрипта. Ако буде било потребе да се подрже старији прегледачи веба, биће коришћен алат [Babel](https://github.com/babel/babel){:target="_blank"}.

- Увлачење: користиће се размаци, а не табови, при чему ће нови ниво увлачења бити маркиран са три размака.

- Тачка-запета: с обзиром на навике настале при програмирању у програмском језику C, усвојена је пркаса да се користи знак тачка-запета на крају сваке наредбе.

- Дужина линије: ако је могуће. линије програмског кŏда пресећи тако да не буду дуже од 80 знакова.

- Линијски коментари: у програмском кŏду користити искључиво линијке коментаре; блоковске коментаре користити искључиво у документационе сврхе.

- Без "мртвог" програмског кŏда: не остављати искоментарисан стари програмски кŏд, како би, "за сваки случај" он могао бити касније коришћен. У оквиру програмског кŏда треба да остане сано садржај који је потребан, а ситуације типа "ово ми може требати касније" се решавају помоћу система за контролу верзија и програмерске документације/напомена.

- Коментарисати само када је корисно: не додавати коментаре ако они не доприносе разумевању програмског кŏда. Ако је коришћењем конвенција кŏдирања, правилним именовањем променљивих и функција програм и коришћењем [JSDoc](https://github.com/google/closure-compiler/wiki/Annotating-JavaScript-for-the-Closure-Compiler){:target="_blank"} коментара постигнуто да програм буде читљив и само-обашњавајући, тада ге не треба додатно коментарисати.

- Именовање функција, променљивих и метода: називи функција, променљивих и метода увек почињу малим словом тј. при запису се користи тзв. **камиљаНотација**. Једино у случају када се ради о називу означеном са `private`, тада назив почиње подвлаком (тј. знаком _ ), а наставак назва је у складу са камиљомНотацијом.

- Именовање конструкторских функција и класа:  називи конструкторских функције и класа користе тзв. **ПаскалНотацију**. И ту се, слично као код камиље нотације, великом словом сигнализира почетак нове речи у називу - само што назив почиње великим, а не малим словом.

- Именовање датотека: називи датотека треба да буду написани малим словима, при чему ће речи у називу бити раздвојене цртицом (или минусмом, тј. знаком - ).

- Константе: све константе се именују **ВЕЛИКИМ_СЛОВИМА**. У том случају се користи подвлаа (тј. знак _ ) за раздвајање речи унутар имена константе.

- Декларације променљивих: увек треба декларисти променљиве, како би се на тај начин избегло "загађивање" стварањем глобалних објеката. При декларисању проеменљивих не користити `var`. Препоручује се коришћењњ `const` за декларацију променљиве, а `let` трба користити само у случају када ће променљивој бити мењана вредност после инцијален доделе.

- Beline: белине треба паметно користити ради повећања читљивости програмског кŏда. На пример, поставити размак иза кључне речи иза које следе отворена заграда; поставити размак пре и после бинарних операција (`+`, `-`, `*`, `/`); после сваке од секција унутар наредбе `for`; после сваког знака тачка-зарез (тј. знака `;`); после сваког зареза (тј. знака `,`), и сл.  

- Знаци за крај линије: убацити празне линије како би се раздвојиле секвенце логички повезаних операција.

- Апострофи и наводници: апостроф (тј. знак `'`) треба да има приоритет у односу на наводник (тј. знак `"`). Наиме, наводници су уобичајени код HTML атрибута, па коришљење апостофа помаже да се олакшају проблеми при раду са нискама које садрже HTML описе.

**Напомена.** Ако радни оквир који се користи или већ усвојени стандард кŏдирањњ садржи другачуја правила, онда се треба њима прилагодити. Један од популарних алата који олакшава сређивање и  форматирање програмског кода је [Prettier](https://prettier.io/){:target="_blank"}.