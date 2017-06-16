%title: illumos, SmartOS, Danube Cloud
%author: Dano a Janči (danubecloud.org)
%date: 2017-06-12

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

-> Zony

-> Dtrace

-> Crossbow (network)

-> SMF

-> Fault Management Facility

-> ...


-------------------------------------------------

-> # BLÍZKE STRETNUTIE S ORACLOM <-


2005: otvorenie Solaris kódu

2007: vyvorenie OpenSolaris distribúcie

2009: odkúpenie Sun-u Oraclom

2010: žiadne info čo bude s OS

2010: Unikol interný dokument o zatvorení kódu
      (Oznámenie nikdy nevyšlo verejne)

2011: Solaris 11 vyšiel bez zdrojových kódov

-------------------------------------------------

-> # 2010: Illumos Odysea <-


Do 90 dní z Oraclu odišla vačšina významných inžinierov
(Tvorcovia ZFS, Dtrace, zón, networking team, ...)

Fork OpenSolaris-u, nazvaný Illumos

Mnohí vývojári skončili v Illumos komunite

Paradox: Oracle nemôže čerpať kód z Illumosu


-------------------------------------------------

-> # DISTRIBÚCIE POSTAVENÉ NA ILLUMOSE <-


SmartOS	     - cloud hypervisor
NexentaStor     - enterprise ZFS storage
OpenIndiana     - desktop
OpenSXCE        - sparc server distro
Dyson           - Debian OS + Illumos kernel
OmniOS          - storage, scalability distro
...

-------------------------------------------------

-> # VÝVOJ POKRAČUJE <-


-> Čo má SmartOS navyše:
-> (cloudový OS)

-> KVM

-> imgadm

-> LX zóny

-> network overlays (vxlan)

-> json integracia

-------------------------------------------------

-> # ZFS <-

-> Enterprise-grade filesystem


-> FS + volume manager

-> Copy on write

-> Snapshoty, prístup k nim

-> ZVOL-s

-> dedup, inline kompresia, ...

-------------------------------------------------

-> # ZÓNY (SOLARIS KONTAJNERY) <-


-> Alternatívy: FreeBSD jails, LXC/Docker

-> Cieľ zón: konsolidácia
-> (security, resource management, bare-metal speed)

-> LX brand

-> Image management + ZFS


-------------------------------------------------

-> # NETWORKING (project Crossbow) <-


-> Plne virtualizované siete
-> (vnics, etherstubs, overlays)

-> QoS, flow control

-> Bezpečnosť

-> Viditeľnosť 

-> Aggr, LACP, IPMP

-------------------------------------------------

-> # DTRACE <-

-> System-wide tracing

-> Minimálne spomalenie aplikácií

-> Viditeľnosť na úroveň C kódu

-> Providers pre vyššie jazyky
-> (python, php, java, ruby, ..)

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

-> Techológie a nápady ostávajú

-> Obojsmerný tok technológií
-> (FreeBSD, Linux, ..)


-> Inovácie netvoria firmy, ale ľudia...

-------------------------------------------------

