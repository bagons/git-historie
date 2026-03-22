# Verzovací systémy

*Verzovací systém je systém, který hlídá a spravuje verze souborů, aby byl přehled v tom co se udělalo, co funguje, co ne atd.*

## Historie

### První verzovací systémy
#### SCCS ([Source Code Control System](https://en.wikipedia.org/wiki/Source_Code_Control_System))

- 1973
- Bell labs

Z nějakého důvodu měl kód tohodle vezovacího systému tenhle string, který ukazoval poslední verzi
```c
static char sccsid[] = "@(#)ls.c        8.1 (Berkeley) 6/11/93";
```
Pak jde údajně najít v binárce podle `@(#)`
#### RCS ([Revision Control System](https://cs.wikipedia.org/wiki/Revision_Control_System))
- pak přebral SCCS
- 1982
- GPL Licence. 
- Udržováno GNU
- Dobře funguje pro jednotlivé soubory, ale podpora několika souborů je omezená.
- Umí větve, ale je to údajně náročný a otravný

#### CVS ([Concurent Versions System](https://en.wikipedia.org/wiki/Concurrent_Versions_System))

- 1986
- využívá RCS
- ale umí Client - Server
- + umí změny na úrovni repozitáře, tedy i několik souborů
- žádné symlinky z bezpečnostních důvodů

*těch verzovacích systémů bylo ještě pár, třeba jako [Subversion](https://en.wikipedia.org/wiki/Apache_Subversion)*