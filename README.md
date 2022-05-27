# TimeMe <img src="https://i.imgur.com/kuPBkLr.png" height="70px" width="70px"> – aplikacija za beleženje opravljenega dela
TimeMe je spletna aplikacija, ki je prvotno namenjena freelancerjem in vsem, ki vsakodnevno delajo na več projektih z različnimi delodajalci. 
S pomočjo TimeMe lahko uporabnik preprosto vodi evidenco opravljenih storitev za posamezne projekte, ki jih sam doda. Ponujen je tudi pregled nad opravljenim delom v obliki poročil in grafov o skupno opravljenem delu ali posameznih delodajalcih.

Uporabnik lahko vsakodnevno vnaša svoja opravila, ponujeni so mu tudi njegovi e-maili in dogodki iz Google Calendar-ja, katere lahko preprosto označi in se vnesejo k izbrani stranki. Vnese lahko tudi dnevne telefonske klice in preostale storitve - opravila, ki niso vezana na trajanje, vendar so obračunana glede na opravljeno storitev, pri katerih lahko izbirate med že vnesenimi šifranti.

# Funkcionalnosti
- vnos projektov
- dodajanje opravil za določen dan in projekt
- dodajanje e-mailov
- dodajanje dogodkov iz Google Calendarja
- dodajanje ročno vnešenih opravil
- dodajanje telefonskih klicev
- dodajanje storitev - tudi po že vnesenimi šifranti
- pregled posameznih projektov
- izračun mesečnega zaslužka glede na vneseno urno postavko
- izpis posameznih vrst v Excel in možnost tiskanja
- kreiranje PDF poročila posameznega projekta
- pregled skupnega dela v obliki grafov

# Tehnološki sklad

|Java EE | JPA | Axios | React | Shards | Recharts | Google Authenticator | Bootstrap | jsPDF-autotable | MUIDataTable
| ------ | ------ | ------ | ------ | ------ |  ------ |  ------ | ------ | ------ | ------ |
| <img src="https://avatars.githubusercontent.com/u/23086798?s=280&v=4" height="50px" /> | <img src="https://hibernate.org/images/hibernate-logo.svg" height="40px" />| <img src="https://user-images.githubusercontent.com/8939680/57233884-20344080-6fe5-11e9-8df3-0df1282e1574.png" height="40px"> | <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/1200px-React-icon.svg.png" height="40px">|<img src="https://avatars.githubusercontent.com/u/8946731?s=200&v=4" height="30px"> | <img src="https://www.richardwestenra.com/painting-with-data-talk/img/libs/recharts.png" height="40px"> |<img src="https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_160x56dp.png" height="40px"> | <img src="https://cdn.icon-icons.com/icons2/2415/PNG/512/bootstrap_plain_logo_icon_146619.png" height="50px"> |<img src="https://www.ap-ps.fr/wp-content/uploads/2019/06/pdf-icon.png" height="40px">|<img src="https://user-images.githubusercontent.com/19170080/34070522-e15d32e2-e235-11e7-8af5-fa704cdcad56.png" height="40px"> |

# Namestitev aplikacije
- Potrebna je namestitev Dockerja (https://www.docker.com/products/docker-desktop).
- Prenesite datoteko Docker (Docker1.zip), ki jo najdete v našem repozitoriju in jo "unzipajte". Pri tem uporabite program, kot je 7Zip ali WinRar, saj ima   Windows pogosto težave z unzipanjem določenih paketov, ki so znotraj Docker mape.
- Odprite PowerShell kot administrator.
- V PowerShell vpišete ukaz: cd mesto Docker datoteke
- V PowerShell vpišete ukaz: docker-compose up
- Če se vam po izvajanju ukaza docker-compose up, prikaže sledeči error (Failed to start service jboss.persistenceunit."delo-backend.war#mysql-pu": org.jboss.msc.service.) morate ponovno napisati ukaz, tako da kliknete ctrl+c (na mac-u Command-C) ter napišete docker-compose up.
- Do React aplikacije se dostopa na localhost:3000, REST strežnik pa na localhost:28080.


# Uporaba aplikacije
Predhodno je treba imeti ustvarjen Google račun, saj je potreben za prijavo. Ker aplikacija zaenkrat še ni potrjena od Googla, mora biti e-mail dodan ročno. Zato se prijavite z testnim Google računom, katerega podatki so navedeni v naslednjem poglavju.
Na začetni strani se prikaže pregled statistike vaših vnešenih mesečnih opravil, kjer lahko vidite v koliko projektih trenutno sodelujete, koliko ur imate opravljenih, kakšen je vaš mesečni zaslužek in še več.

<img src="https://imgur.com/TwB9GNh.png" width="400px"/>

S klikom na "Vnos projekta" lahko izpolnite vnosna polja in dodate nov projekt, na katerem delate. Vpišete lahko tudi elektronske naslove in telefonske številke strank. 

Na seznamu vseh projektov si lahko ogledate vse trenutne projekte, s klikom na "Ogled podrobnosti" pa pridobite povzetek celotnega projekta v obliki tabel po različnih vrstah opravil. Posamezno si lahko tako izvozite npr. telefonske klice, e-maile, ročno vnesena opravila itd. v Excel ali jih natisnete.

<img src="https://imgur.com/7EwZ6P0.png" width="400px" />

Ustvarite lahko tudi PDF poročilo o posameznem projektu na mesečni ravni.

Da dodate posamezno opravilo kliknete na "Vnos opravila". Najprej izberete projekt in datum, za katerega vnašate opravilo. Nato sledite puščicam, ki vas vodijo po dodajanju e-mailov, ročno dodanih opravil, dogodkov iz Google Calendarja, telefonskih klicev in storitev. Storitve lahko dodajate tudi po že obstoječih šifrantih.
Pri enem vnosu opravila lahko dodate več posameznih opravil s pomočjo gumba "Shrani". Opravila se vam bodo prikazala spodaj na posamezni strani, na koncu pa bo možen pregled vseh dodanih opravil.

<img src="https://imgur.com/0SD245T.png" width="400px" />
<img src="https://imgur.com/DIGn9SO.png" width="400px" />


# Testni Google račun

- Mail: time.me.help@gmail.com
- Geslo: FeriJeFajn123

# Podatki o Google API project-u

- Ime Google projekta: PraktikumDva
- Console name: Delo
- Client Id: 527793511850-buh61dvqku6kah3t3qo926bs7odsfag2.apps.googleusercontent.com
- Client secret: 0OP3EvOQA-LWdyRStfybGUxU
- API key: AIzaSyDwsQDgMcBsrsvCBjT8AYNxVksZ-XpXmNI

# Diagram primerov uporabe

![DPU](Diagrami/DPU.png)

# Avtorji
@ZigaPigac
@IremIsmail
@tilenRojko
@tjasamalok

<img src="https://i.imgur.com/cPYfNpa.png" width="1200px" />
