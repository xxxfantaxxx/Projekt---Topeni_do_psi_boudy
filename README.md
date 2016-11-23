14.9.2016
Ročníkový projekt IT4

#Topení do psí boudy

O vyhřívání neboli temperování psí boudy jsou na internetu jen zmínky že je to možné. Žádné podrobnější informace o realizaci takové boudy jsem nikde nenašel. Maximálně je zmínka o topných rohožích. Topné rohože, nebo kabely existují. Jejich nespornou výhodou je možnost tzv. seberegulace. Některé typy kabelů, které se používají jako ochrana proti zamrznutí potrubí,okapů,schodů, mají tu dobrou vlastnost, že pracují automaticky.(mají v sobě protizámrazovou regulaci)Jejich alespoň pro mne zásadní nevýhodou je cena těchto systémů a taky skutečnost, že jsou vyráběny ve velikostech a výkonově podstatně větší než je naše potřeba.Samozřéjmě lze si nechat udělat topný kabel na míru. Já jsem se rozhodl a to především z důvodů pořizovacích nákladů pro vlastní řešení.

Jako zdroj tepla, mám v plánu využít "špatnou" vlastnost žárovky.A to že účinost žárovky je někde kolem 11%. Zbytek dodané energie se mění v teplo.Jako další důležitý klad tohoto zdroje je možnost volbou typu žárovky zvolit optimální výkon topné jednotky (Klasická žárovka E27 se vyrábí v řadě 230V/25W 40W 60W 75W 100W).Pro temperování dobře zateplené ložnice potřebujeme opravdu minimální příkon.Cena žárovky nepřekročí 30 Kč. Nic ovšem není zase tak jednoduché a proto i toto řešení má své nedostatky.

Zdroj tepla

Jako zdroj tepla jsem využil "špatnou" vlastnost žárovky.A to že účinost žárovky je někde kolem 11%. Zbytek dodané energie se mění v teplo.Jako další důležitý klad tohoto zdroje je možnost volbou typu žárovky zvolit optimální výkon topné jednotky (Klasická žárovka E27 se vyrábí v řadě 230V/25W 40W 60W 75W 100W).Pro temperování dobře zateplené ložnice potřebujeme opravdu minimální příkon.Cena žárovky nepřekročí 10 Kč. Nic ovšem není zase tak jednoduché a proto i toto řešení má své nedostatky.

Žárovka když topí tak i svítí.

Povrch žárovky dosahuje za provozu velkých teplot

Životnost žárovky v uzavřeném prostoru???

Konstrukce a montáž: první problém vyřeším tím, že žárovku uzavřu do kovové trubky. Tím dosáhnu toho, že světlo není vidět a zároveň je to ochrana při případném prasknutí a rozsypání baňky žárovky.

Povrch trubky dosahuje za provozu velkých teplot. Proto musí být topná patrona chráněna krytem ze všech stran!!! Mohlo by dojít k popálení psa, případně ke vzniku požáru, kdyby se patrona dostala do styku s kobercem,nebo podestýlkou která je uvnitř boudy! Taktéž celá jednotka je namontována na stěně ložnice se vzduchovou mezerou!

Jako poslední možná nevýhoda je zkrácení životnosti žárovky s ohledem na její špatné ochlazování. To je sice fakt, ale při ceně žárovky tento argument postrádá smysl. Pokud vezmeme klasickou přenosku, nebo sklepní světla s krytím IP44 ty jsou také utěsněna a sklo je špatný tepelný vodič. V našem případě je výhodné použít pro výrobu patrony co možná největší a nejdelší trubku (trubka není podmínkou). Tím dosáhneme větší plochy pro vyzařování tepla a tím snížíme tepelnou zátěž pro žárovku.
Náklady na materiál potřebný pro výrobu topné jednotky je zanedbatelný a dá se sehnat ve šrotě.


#Použité knihovny(libraries)
UTFT.h[Absolute README link](https://github.com/xxxfantaxxx/Projekt---Topeni_do_psi_boudy/blob/master/Termostat/code2_zaklad_menu)

EEPROM.h[Absolute README link](https://github.com/xxxfantaxxx/Projekt---Topeni_do_psi_boudy/blob/master/Termostat/code2_zaklad_menu)

Wire.h[Absolute README link](https://github.com/xxxfantaxxx/Projekt---Topeni_do_psi_boudy/blob/master/Topeni-primo_na_boude/zkouska_I2C)

LiquidCrystal.h[Absolute README link](https://github.com/xxxfantaxxx/Projekt---Topeni_do_psi_boudy/blob/master/Topeni-primo_na_boude/code1_zaklad_nastaveni_teploty)

#Schémata a použité materiály

první pracovní schéma Termostatu(Arduino mega, lcd touch display, rf 433 mhz(radiová komunika pro odesílání i příjmání))
![received_1291220147595396](https://cloud.githubusercontent.com/assets/14974350/19142641/3c7f44ec-8b9f-11e6-8693-8e2bcb942ce1.jpeg)

čip pro rádiovou komunikaci(na schématu nahoře vpravo)

![fdmy7jthm8dg3ph medium](https://cloud.githubusercontent.com/assets/14974350/19142947/401bd17c-8ba1-11e6-80c1-0ff7fb94d4c0.jpg)

lcd touch display(na schémau vpravo)

![htb1ildrlfxxxxxbxxxxq6xxfxxxl](https://cloud.githubusercontent.com/assets/14974350/19143204/9627e014-8ba2-11e6-89b5-8fa296c544ab.jpg)

arduino mega (na shcématu vlevo)
![htb1ylrdkvxxxxcjxvxxq6xxfxxxu](https://cloud.githubusercontent.com/assets/14974350/19143258/0404e280-8ba3-11e6-9578-3fdbf0859e86.jpg)


TFT 3.2 inch Mega Touch LCD Expansion Board Shield(pro spojení arduina(mega) a dotykového dispalye)
![htb1bfrwkvxxxxbexfxxq6xxfxxxs](https://cloud.githubusercontent.com/assets/14974350/19143160/4977bed8-8ba2-11e6-9207-91dca2cf2fc2.jpg)


Zde vidíme Arduino nano 3.0 které bude použito pro chod "topení"
![1pcs-nano-3-0-controller-compatible-with-nano-ch340-usb-driver-no-cable-for-arduino-nano](https://cloud.githubusercontent.com/assets/14974350/19126237/5fd38e22-8b3a-11e6-9399-a80803683ea7.jpg)


NOVÉ SCHÉMA!!!!!! termostat na boudě s relátkem ke spuštění topení
![termostat_bouda](https://cloud.githubusercontent.com/assets/14974350/19507637/91bfa8cc-95d4-11e6-9ac6-fcc04799b1bd.png)


         
 
