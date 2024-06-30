https://github.com/Donsonsoft/EMD

---------------------------------------------------------
Komu je tento projekt určený?
Napríklad každému, kto si svoje heslá len tak ukladá do textového súboru. Či už zdieľate počítač s druhou osobou, alebo heslá ukladáte zvlášť na externé úložisko, vždy je vhodné uchovávať ich zašifrované. Nezašifrované heslá v elektronickej podobe sú relatívne ľahko ukradnuteľné. Zašifrovaním svojich citlivých údajov vo forme textu predídete ich zneužitiu.
---------------------------------------------------------

---------------------------------------------------------
VÝHODY
- na šifrovanie ani na dešifrovanie nepotrebujete pripojenie k internetu - všetko sa vykoná priamo vo vašom webovom prehliadači
- šifrovací program je open-source - môžete ho študovať, upravovať (neodporúčam neodborne upravovať javascript) a pozmenený voľne zdieľať, no nezabudnite "svoje dielo" podpísať, aby ľudia vedeli, že program je upravený
- pôvodný text (tzv. otvorený text) nie je po zašifrovaní nikde uložený (po reloade stránky ani v textovom poli)
---------------------------------------------------------

---------------------------------------------------------
OBMEDZENIA
- Program nedokáže pracovať so všetkými znakmi (viď abecedy.txt).
- Program nedokáže pracovať s netlačiteľnými znakmi (no medzery dokáže skonvertovať na podčiarkovníky "_")
- Ak má otvorený text viac riadkov (resp. odsekov), musia byť skonvertované na špecifický znak (predvolený je ;), aby bolo možné ich obnoviť pri dešifrovaní
---------------------------------------------------------

---------------------------------------------------------
VÝSTRAHA!

Ja, autor, nezodpovedám za žiadne straty vašich údajov. Dobrovoľne ste sa rozhodli používať môj program a je len na vás, či si zapamätáte šifrovací kľúč, prípadne či nestratíte vlastné abecedy.
Pozor na zmeny verzií šifry EMD! Ak zašifrujete text v nižšej verzii napr. 1.0 a pokúsite sa ho dešifrovať vo verzii 2.2, nedostanete pôvodný text! Dôležité je prvé číslo - to udáva verziu šifrovacieho algoritmu, čísla za bodkou značia opravy v dizajne alebo nejakej funkcionalite, prípadne značia pridanie funkcionality. Takže text zašifrovaný verziou 2.0 môže byť dešifrovaný verziou 2.2.
---------------------------------------------------------

---------------------------------------------------------
POUŽITIE

Šifrovanie

0. Zožeňte si text, ktorý chcete zašifrovať :-)
1. Prilepte (prípadne vpíšte) svoj text do príslušného textového poľa
2. Vymyslite si bezpečný šifrovací kľúč (heslo), ktorý vpíšte do príslušného poľa
3. Kliknite na tlačidlo "Zašifruj"

Dešifrovanie

0. Zožeňte si text, ktorý chcete dešifrovať :-)
1. Prilepte svoj text do príslušného textového poľa
2. Vspomente si na svoj šifrovací kľúč (heslo), ktorý vpíšte do príslušného poľa
3. Kliknite na tlačidlo "Dešifruj"

- môžu sa objaviť rôzne chybové hlásenia a zároveň funkcie na opravu niektorých chýb (nahradenie medzier alebo značiek odseku)
- kľúč môžete zobraziť kliknutím na začiarkovacie políčko
- je možné použiť aj vlastné abecedy, ktoré zvýšia bezpečnosť šifrovania (viac info nižšie)
- nezašifrovaný aj zašifrovaný text môžete skopírovať do schránky pomocou modrých guľôčok po pravej strane textových polí
---------------------------------------------------------

---------------------------------------------------------
OBSAH ZIP SÚBORU

- readme.txt je tento uvádzací text :-)
- sifra_emd.html je samotný šifrovací program spustiteľný prostredníctvom akéhokoľvek webového prehliadača (aj v mobile), nič iné na šifrovanie nepotrebujete
- abecedy.txt je súbor s predvolenými abecedami, slúži len ako vzor pre vaše vlastné abecedy (pre funkčnosť programu je nepodstatný)
---------------------------------------------------------

---------------------------------------------------------
VLASTNÝ SÚBOR S ABECEDAMI (nepovinný)

Vo verzii 2.2 pribudla funkcionalita na vytvorenie vlastných abecéd bez námahy. Stačí kliknúť, uložiť a použiť.

Vlastnosti súboru s abecedami:

- obsahuje 128 riadkov a v každom z nich 128 znakov
- použité sú nasledovné znaky v náhodnom poradí (znaky sa v riadku neopakujú):
aáäbcčdďeéfghiíjklĺľmnňoóôpqrŕsštťuúvwxyýzžAÁÄBCČDĎEÉFGHIÍJKLĹĽMNŇOÓÔPQRŔSŠTŤUÚVWXYÝZŽ0123456789+-*/^<=>,.;:?!_§$€#&@{}[]()~|%¦˚

Aký má zmysel používať vlastné abecedy?
Program má aj svoje predvolené abecedy, takže sa o nič neukrátite, ak vlastné abecedy nepoužijete.
No ak použijete vlastné abecedy, markantne zvýšite bezpečnosť svojich dát (ak ich samozrejme nenecháte na očiach potenciálnemu útočníkovi).
Ak použijete slabý kľúč (napr. meno svojho psa) útočník môže heslo prelomiť tzv. hrubou silou, no s použitím súboru s abecedami mu takýto útok znemožníte (ak sa mu nedostane do rúk)
Vytvorením vlastných abecéd vlastníte unikátny súbor, ktorý je na jednu stranu nepraktický, keďže ho musíte mať so sebou pre potrebu dešifrovania, no je omnoho bezpečnejší.
Je to vlastne 16384 znakové, unikátne heslo, preto je tak bezpečné.
---------------------------------------------------------
