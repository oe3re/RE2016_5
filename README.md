# RE2016_5
Šifrovanje- projekat 5


Napisati program koji kodira tekst koji se kuca na tastaturi Playfair-ovom šifrom. Prilikom
kucanja poruke na standardnom izlazu se prikazuje šifrovana poruka.
Playfair-ovo šifrovanje zamenjuje grupu od dva znaka abecede grupom od dva znaka po sledećem
algoritmu. Konstruiše se 5×5 matrica slova koja će u našem zadatku biti:
P L A Y F
IJ R B C D
E G H K M
N O Q S T
U V W X Z,
a zatim se podeli tekst na blokove od po dva slova (bez blanko znakova) koji se koduju na tri
moguća načina:
• Slova se nalaze u istom redu. Tada ih zamenimo sa slovima koja se nalaze za jedno mesto
udesno (ciklično). Npr. EH → GK, ST → TN, FP → PL.
• Slova se nalaze u istoj koloni. Tada ih zamenimo sa slovima koja se nalaze za jedno mesto
ispod (ciklično). Npr. OV → VL, KY → SC, PI → IE.
• U protivnom, pogledamo kvadrat koji određuju ta dva slova, pa ih zamenimo s preostala
dva vrha tog kvadrata. Redosled je određen tako da prvo dolazi ono slovo koje se nalazi
u istom redu kao prvo slovo u polaznom bloku. Npr. OC → SR, RK → CG, PD → FI.
Znakovi I i J se poistovećuju.
