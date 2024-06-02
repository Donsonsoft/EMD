# EMD
EMD is my own encryption program which is already quite secure and usable in my opinion
This file is currently written in slovak language only.

---------------------------------------------------------
Komu je tento projekt určený?
Napríklad každému, kto si svoje heslá len tak ukladá to textového súboru.
Nezašifrované heslá v elektronickej podobe sú relatívne ľahko ukradnuteľné.
Zašifrovaním svojich citlivých údajov vo forme textu zvýšite bezpečnosť svojich uložených hesiel.
---------------------------------------------------------

---------------------------------------------------------
OBMEDZENIA
- Program nedokáže pracovať so všetkými znakmi (viď abecedy.pdf).
- Program nedokáže pracovať s netlačiteľnými znakmi (no medzery dokáže skonvertovať na podčiarkovníky "_")
- Ak má otvorený text viac riadkov (resp. odsekov), musia byť skonvertované na špecifický znak (predvolený je ;), aby bolo možné ich obnoviť pri dešifrovaní
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
- logika.pdf slúži len pre pochopenie činnosti môjho algoritmu (pre funkčnosť programu je nepodstatný)
- abecedy.txt je súbor s predvolenými abecedami, slúži len ako vzor pre vaše vlastné abecedy (pre funkčnosť programu je nepodstatný)
- abecedy_demo.txt je druhý variant abecéd, ktorý môžete použiť pri šifrovaní, no prednostne slúži ako vzor (pre funkčnosť programu je nepodstatný   za predpokladu, že ho nechcete používať)
- abecedy.pdf obsahuje hlavnú abecedu a predvolené abecedy (pre funkčnosť programu je nepodstatný)
---------------------------------------------------------

---------------------------------------------------------
VLASTNÝ SÚBOR S ABECEDAMI (nepovinný)
- musí obsahovať 128 riadkov a v každom z nich 128 znakov
- Dôležité je, aby každý riadok obsahoval všetky nasledovné znaky a aby v každom riadku boli v náhodnom poradí:
aáäbcčdďeéfghiíjklĺľmnňoóôpqrŕsštťuúvwxyýzžAÁÄBCČDĎEÉFGHIÍJKLĹĽMNŇOÓÔPQRŔSŠTŤUÚVWXYÝZŽ0123456789+-*/^<=>,.;:?!_§$€#&@{}[]()~|%¦˚

Odporúčam tento online nástroj na zamiešanie písmen: https://codebeautify.org/shuffle-letters
Tieto znaky sú zároveň všetky znaky, ktoré môžete použiť v šifrovacom kľúči a v otvorenom texte (nezašifrovaný text).

Keby ste chceli použiť aj iné znaky, museli by ste zmeniť hlavnú abecedu priamo v programe napísanom v jazyku JavaScript. Upravovať zdrojový kód neodporúčam, aby ste omylom nezmenili funkčnosť programu a aby ste program neznefunkčnili.
Vyhnite sa úvodzovkám (" a ') a hlavne spätnému lomítku (\), ktoré sa používa v jazyku JavaScript.

Aký má vôbec zmysel vytvárať vlastné abecedy?
Program má aj svoje predvolené abecedy, takže sa o nič neukrátite, ak vlastné abecedy nepoužijete.
No ak vytvoríte vlastné abecedy, markantne zvýšite bezpečnosť svojich dát (ak ich samozrejme nenecháte na očiach potenciálnemu útočníkovi).
Šifrovací kľúč je samozrejme tiež potrebný na dešifrovanie, no ak použijete slabý kľúč (napr. meno svojho psa) je možné dešifrovať dáta tzv. hrubou silou.
Použitím vlastných abecéd vytvoríte unikátny súbor, ktorý je na jednu stranu nepraktický, keďže ho musíte mať so sebou pre potrebu dešifrovania, no je omnoho bezpečnejší.
Je to vlastne 16384 znakové, unikátne heslo, preto je tak bezpečné.

---------------------------------------------------------
