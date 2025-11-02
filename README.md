# openbox-python3.14-fix  
Aquest repositori resol un bloqueig funcional d'Openbox amb Python 3.14.

Evita errors d'AST i SyntaxWarning al menú dinàmic.

S'han identificat incompatibilitats que impedien generar el menú dinàmic. Aquest projecte aplica les correccions necessàries per restaurar el funcionament en entorns actuals.

## Arxius modificats

Les correccions s'han aplicat als següents arxius del sistema:

- `Menu.py`  
  → Ubicació: `/usr/lib/python3.14/site-packages/xdg/Menu.py`  
  → Arxiu Python que genera el menú dinàmic.  
  → S'ha corregit la sintaxi per adaptar-la a Python 3.14 i evitar errors d'AST.

- `openbox-xdg-menu`  
  → Ubicació: `/usr/libexec/openbox-xdg-menu`  
  → Script auxiliar que integra el menú dinàmic amb Openbox.  
  → S'ha ajustat per garantir compatibilitat amb el nou `Menu.py`.

Repositori mantingut per [Joan](https://github.com/siette).
