%title: illumos, SmartOS, Danube Cloud
%author: Ján Poctavek, Daniel Kontšek (danubecloud.org)
%date: 2017-06-18

mdp
===

-> A command-line based markdown presentation tool. <-

_Basic controls:_

next slide      *Enter*, *Space*, *Page Down*, *j*, *l*,
                *Down Arrow*, *Right Arrow*

previous slide  *Backspace*, *Page Up*, *h*, *k*,
                *Up Arrow*, *Left Arrow*

quit            *q*
reload          *r*
slide N         *1..9*
first slide     *Home*, *g*
last slide      *End*, *G*

-------------------------------------------------

-> # HISTÓRIA SOLARISU <-


1983: SunOS 1.0  (BSD 4.1)

1994: SunOS 4.1.4  (BSD 4.3)

1991: System V Release 4 (BSD + System V + Xenix)

1992: SunOS 5.0 = Solaris 2.0  (SVR4)


-------------------------------------------------

-> # ZLATÝ VEK SOLARISU (2001 - 2009) <-


-> Stabilný OS + anarchia vo firme =
<br>

-> ZFS

-> Zóny

-> Dtrace

-> Crossbow (network)

-> SMF

-> Fault Management Facility

-> ...


-------------------------------------------------

-> # BLÍZKE STRETNUTIE S ORACLOM <-


2005: otvorenie Solaris kódu

2007: vytvorenie OpenSolaris distribúcie

2009: odkúpenie Sun-u Oraclom

2010: žiadne info čo bude s OS

2010: unikol interný dokument o zatvorení kódu
      (oznámenie nikdy nevyšlo verejne)

2011: Solaris 11 vyšiel bez zdrojových kódov

-------------------------------------------------

-> # 2010: ILLUMOS ODYSEA <-


Do 90 dní z Oraclu odišla väčšina významných inžinierov.
(Tvorcovia ZFS, Dtrace, zón, networking tím, ...)

Fork OpenSolaris-u, nazvaný *illumos*.

Mnohí vývojári skončili v illumos komunite.

Paradox: Oracle nemôže čerpať kód z illumosu.


-------------------------------------------------

-> # DISTRIBÚCIE POSTAVENÉ NA ILLUMOSE <-


OpenIndiana     - server, desktop
SmartOS	     - cloud hypervisor
NexentaStor     - enterprise ZFS storage
OpenSXCE        - sparc server distro
Dyson           - Debian OS + illumos kernel
OmniOS          - storage, scalability distro
...

-------------------------------------------------

-> # VÝVOJ POKRAČUJE <-


-> Čo má SmartOS navyše:
-> (cloudový OS)

-> KVM

-> imgadm

-> LX zóny

-> network overlays (VXLAN)

-> JSON integrácia

-------------------------------------------------

-> # ZFS <-

-> Enterprise-grade filesystem


-> FS + volume manager

-> Copy on write

-> Snapshoty, prístup k nim

-> ZVOL-s

-> deduplikácia, inline kompresia, ...

-------------------------------------------------

-> # ZÓNY (SOLARIS CONTAINERS) <-


-> Alternatívy: FreeBSD jails, LXC/Docker

-> Cieľ zón: konsolidácia
-> (security, resource management, bare-metal speed)

-> LX brand, Docker

-> Image management + ZFS


-------------------------------------------------

-> # NETWORKING (project Crossbow) <-


-> Plne virtualizované siete
-> (VNICs, etherstubs, overlays)

-> QoS, flow control

-> Bezpečnosť

-> Viditeľnosť 

-> Agregácia liniek, LACP, IPMP

-------------------------------------------------

-> # DTRACE <-

-> System-wide tracing

-> Minimálne spomalenie aplikácií

-> Viditeľnosť na úroveň C kódu

-> Podpora pre vyššie jazyky
-> (Python, PHP, Java, Ruby, ...)

-> Štatistické funkcie

-> Dtrace toolkit

-------------------------------------------------

-> # KVM + QEMU <-

-> Preportované z Linuxu

-> To najlepšie z oboch svetov:

-> Networking
-> Dtrace
-> Bezpečnosť zón
-> ZFS zvols
-> imgadm

-------------------------------------------------

-> # DEDIČSTVO SOLARISU <-


-> Budúcnosť ukáže

-> Technológie a nápady ostávajú

-> Obojsmerný tok technológií
-> (FreeBSD, Linux, ...)


-> Inovácie netvoria firmy, ale ľudia...

-------------------------------------------------

-> # DANUBE CLOUD <-

Open source *software* na správu
cloudovových datacentier.


Agenda
------

História Erigones / Danube Cloud

Vlastnosti Danube Cloud

Demo

Vývoj a open source

Záver / Diskusia

-------------------------------------------------

-> # HISTÓRIA ERIGONES / DANUBE CLOUD <-


Systémový administrátor

Objavenie SmartOS-u

Python, distribuovaný manažment úloh

`Cieľ`: Sústredenie sa na používateľov a
      služby namiesto opakovaných úloh


-------------------------------------------------

-> # VLASTNOSTI DANUBE CLOUD <-


Rýchle a jednoduché nasadenie

SmartOS hypervisor

Virtuálne datacentrá (multi-tenancy)

Integrovaný monitoring (Zabbix), DNS, IP plán

Rýchle snapshoty VM a zálohovanie


-------------------------------------------------

-> # DEMO <-

-------------------------------------------------

-> # VÝVOJ A OPEN SOURCE <-


Cesta k open source

Používateľská príručka

Nástroj na výrobu image-ov

Význam OSS pre vývojárov

-------------------------------------------------

-> # ZÁVER A DISKUSIA <-


Homepage: danubecloud.org

User guide: docs.danubecloud.org

Development: github.com/erigones/esdc-ce/wiki

Contact: dc@erigones.com

Spojte sa s nami:
-----------------
- facebook.com/DanubeCloud
- twitter.com/DanubeCloud
