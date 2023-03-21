# dndmagicitems
dnd maagiliste esemete jaoks andmebaasi
Link: https://gitmind.com/app/docs/mytwvaac
https://dbdesigner.page.link/L7G3qsVDSS6rNYtQA
Password: 7497


Relatsioonid ja reeglid:
Generaatoris asub nimetatud itemid, millele on antud enda id, efekti id ja baas itemi id

RELVAD:

Id - igale oma id integer

DMG_TÜÜP - baasrelvadel kas piercing (prc), slashing (sls), bludgeoning (bld)

Relva hind - vaskmüntides positiivne integer (10 cp= 1 sp, 10 sp = 1 gp)

Relva omadused - valik listist {Finesse, Heavy, Light, Loading, Range, Reach, Thrown, Two-Handed, Versatile}

Kategooria - valik {martial,simple}

Range - {x,y}, kui on melee siis on {0,0}, thrown properiga relvadel on siin ka range nagu ammunition omadel.

dmg - {x}d{y} kus x on täringute arv ja y on täring valikust {4,6,10,12,20,100}


KASUTATAVAD:

Id - igale oma


hind - vaskmüntides positiivne integer (10 cp= 1 sp, 10 sp = 1 gp)

kordarv - mitu korda saab kasutada

võimsus - integer mitu korda efekti täringuid korrutada

omadused - {drink,single target,AOE}

ala - kui AOE, siis positiivne integer (ringala mis mõjutab)


MUUD ESEMED:

Id - igale oma

tüüp - asja nimi

hind - vaskmüntides positiivne integer (10 cp= 1 sp, 10 sp = 1 gp)

omadused - {wearable,held} kas riideese v midagi muud

ala - kui AOE, siis positiivne integer (ringala mis mõjutab)


TURVISED:

Id- igale oma

hind - vaskmüntides positiivne integer (10 cp= 1 sp, 10 sp = 1 gp)

raskus - {heavy,medium,light}

AC - baas ac ilma dex lisamiseta

stealth - {true,false} näitab itemi disadvantagi


=============================================================================

EFEKTID:

Id - igale oma

nimi - efekti nimi

tüüp - {BUFF,DMG,DEBUFF,UTILITY,HEAL}

hind - hind mis lisada baas itemi hinnale

omadused - kirjeldab mis teeb

täring - HEAL ja DMG puhul palju formaadis xdy+mod {x-mitu,y-kui suur, mod-kui palju baas enne täringu veeretust}


=============================================================================

EELGENEREERITUD:

Id - igale oma

NIMI - ühendab efekti ja baasitemi nime

Item Id - baas itemi id

Efekt Id - baas efekti id




Tuleb teha selgeks kuidas genereerimine käib, eelgenereeritud on need millest efektid saadud, ühendatud tüübid, genereeritud itemitele vahetabel kus baas item mitte baas relv vms.
