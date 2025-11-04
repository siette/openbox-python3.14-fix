# openbox-python3.14-fix  
Aquest repositori resol un bloqueig funcional d'Openbox amb Python 3.14.

Evita advertiments de sintaxi i incompatibilitats amb Python 3.14 al menú dinàmic.

S'han identificat incompatibilitats que impedien generar el menú dinàmic. Aquest projecte aplica les correccions necessàries per restaurar el funcionament en entorns actuals.

## Arxius modificats

Les correccions s'han aplicat als següents arxius del sistema:

- `Menu.py`  
  → Ubicació: `/usr/lib/python3.14/site-packages/xdg/Menu.py`  
  → Arxiu Python que genera el menú dinàmic.  
  → S'ha corregit la sintaxi per adaptar-la a Python 3.14, segons els requisits del llenguatge en aquesta versió.
    El codi original funcionava correctament en versions anteriors, però Python 3.14 exigeix una escriptura diferent en alguns casos.

- `openbox-xdg-menu`  
  → Ubicació: `/usr/libexec/openbox-xdg-menu`  
  → Script auxiliar que integra el menú dinàmic amb Openbox.  
  → S'ha ajustat per garantir compatibilitat amb el nou `Menu.py`.

Pot funcionar amb altres versions 3.x, però no s'ha provat.

Repositori mantingut per [Joan](https://github.com/siette).


## Llicència

Aquest projecte està sota la GNU General Public License, versió 2 o superior (GPLv2+).

El fitxer `openbox-xdg-menu` manté la llicència GPLv2+ original de Red Hat.

Pots consultar el text complet de la llicència al fitxer [LICENSE](./LICENSE).

