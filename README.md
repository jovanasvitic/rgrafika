# 
Projekat iz predmeta Računarska grafika

Izrada projekta se sastoji iz dve faze. Prva faza podrazumeva modelovanje statičke 3D scene. U to se ubraja kreiranje prozora, testiranje dubine i sakrivanje nevidljivih površina. Najvažniji deo prve faze je učitavanje, modelovanje i prikaz mesh modela. Druga faza podrazumeva definisanje materijala, osvetljenja, tekstura, interakcije i kamere u 3D sceni. Prvo treba definisati svetlosni izvor u skladu sa zahtevima zatim učitati, dodeliti, podesiti i mapirati teksture, nakon toga definisati kameru. Sledeći korak je da se omogući interakcija sa korisnikom pomoću kontrole korisničkog interfejsa i tastera. Kao krajni korak treba realizovati animaciju transformacijom sveta ili korišćenjem gluLookAt() metode.
Korišćen je OpenGL - standardni programski interfejs aplikacije namenjen razvoju aplikacija iz oblasti 2D i 3D grafike. Implementacija OpenGL standarda postoji za veliki broj platformi. To je intuitivan i jednostavan interfejs koji omogućava razvoj aplikacija sa manjim programerskim naporom. OpenGL se sastoji od iz dva dela, prvi propisuje funkcionalnosti dok drugi deo podrazumeva da se ta funkcionalnost implementira. Aplikacija poziva metode a server ih izvršava. 
OpenGL implementacija koja je korišćena organizovana je kao programerska biblioteka SharpGL. Na Windows platformi funkiconalanost osnovne biblioteke je implementirana u SharpGL.dill dinamičkoj programskoj biblioteci. 

Projektni zadatak - Trka bolida Formule 1

Importovana su dva različita modela bolida Formule 1. Modelovane su podloga, staza i zaštitni zidovi sa leve i desne strane staze, korišćenjem instanci Cube klase. Metodom glColor definisana je ambijentalna i difuzna komponenta materijala. Definisan je tačkasti svetlosni izvor svetložute boje, pozicioniran gore-levo u odnosu na centar scene i stacioniran. Podešeni su filteri za teksturu na linearno filtriranje. Način stapanja teksture sa materijalom je GL_DECAL. Teksture pridružene stazi, zidovima i podlozi(asfalt, metalna ograda, šljunak) su skalirane pomoću Texture matrice. Kamera je pozicionirana tako da gleda scenu spreda i odgore. Mogućnosti interakcije sa korisnikom su transliranje desnog bolida po horizontalnoj osi, rotiranje levog bolida oko vertikalne ose i izbor boje ambijentalne komponente izvora. Kreirana je animacija u kojoj leva formula od starta vodi i pobeđuje, a kamera prvo zumira stazu a zatim prelazi na kadar odgore.

Pokretanje

Aplikacija se otvara u VisualStudiu, pokreće se samo klikom na dugme Start. Interakcija preko tastature: sa F4 izlazi se iz aplikacije; tasterima +/- vrši se približavanje i udaljavanje od centra scene; tasterima I/K vrši se rotacija oko horizontalne ose; tasterima J/L vrši se rotacija oko vertikalne ose; animacija se pokreće na taster V;
