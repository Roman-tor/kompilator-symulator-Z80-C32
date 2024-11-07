kompilator procesora Z80, wraz z symulatorem Z80. W pliku <programy> jest plik nowy.asm jak przykład
kompilator symulator - autorzy: Marat Fayzullin i  mgr inż. J. Rydzewski (Politechika Białostocka)
Kpmpilator działa pod systemem 32-bit owym , nie trzeba go instalować, wystarczy otworzyć plik hex. Jeśli masz np. WIN 64-bit, 
można zaistalować wirtualną maszynę / ja mam Oracle VM Virtual Box/ i w tej maszynie zainstalować np. WIN XP 32-bit, może byc inny
ale XP nie zajmuje tyle miejsca co np. 7 czy wyższy a XP w zupełności wystarczy do  tego kompilatora
Zaletą tego kompilatora jest to, że można przed kompilacją wczytać plik HEX i wykonać kompilacje pliku ASM. Kompilacja zmieni
tylko bajty wg pliku ASM, nie naruszając pliku HEX chyba, że adresy po kompilacji sa "wewnątrz" pliku HEX. Daję to możliwośc 
dodawania pliku HEX do istniejącego. Np. mamy oryginał pliku HEX "MONITORA" CA80 /od 0h do 1FFFh/, piszemy jakiś plik ASM 
od 2000h, kompilujemy i mamy wynikowy plik HEX z naszym programem z pliku ASM. Musimy tylko teraz go zapamiętać /czwarta ikonka/.
Drugą ważną zaletą jest symulacja pracy naszego programu: krok po kroku, można przeskoczyć procedurę, np. CALL XY lub wykonać 
podprocedurę - tylko do RET. Widoczne są też wszystkie rejestry procesora, można też odcztać czas wykonywania symulacji! 
Opis w pliku "opis_symZ80.pdf" i "metaasembler.pdf"

BŁędy podczas kompilacji możemy "znaleźc" np. edytując plik LST w notatniku - odczytać adres z literką V /np. VC000/, zapamiętać
nr wiersza i odnaleźć ten nr wiersza w edytownym aktualnie pliku ASM kompilatora. Nie ma możliwości sprawdzenia prawidłowosci
"syntax" / składnia języka programowania/ przed kompilacją! Kompilator ASide ma taką możliwość.

inny kompilator do procesora Z80 , w wersji  niemieckiej /Shareware/ 
ASide można ściągnąć z
http://www.theeg.de/aside/index.html - wersja niemiecka Shareware
