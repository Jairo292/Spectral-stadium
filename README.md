\# 🏟️ Spectral Stadium – Entregable 2



\### Rama: `feature/entregable2-checkpointB`



Este segundo entregable corresponde al desarrollo e integración de las principales funcionalidades del proyecto \*\*Spectral Stadium\*\*, incluyendo jugabilidad, IA, sistemas visuales, inventario y menús interactivos.



---



\## 🎮 1. Jugabilidad y personaje principal



\- Reemplazo del personaje principal por \*\*NewGuard\*\*, con su propio set de animaciones personalizadas.

\- Implementación de \*\*barra de vida (Health Bar)\*\* mediante `Widget Blueprint`.

\- \*\*Control dual:\*\* soporte tanto para \*\*teclado\*\* como \*\*gamepad\*\*.

\- Ajustes de movimiento y cámara adaptados al nuevo personaje.



📂 \*\*Ubicación:\*\*  

`Content/ThirdPerson/Blueprints/`  

`Content/jdma/Models/newguard/`



---



\## 🧠 2. IA básica para NPCs



\- Creación de un sistema de inteligencia artificial con:

&nbsp; - \*\*Behavior Tree (`BT\_NPC`)\*\*

&nbsp; - \*\*Blackboard (`BB\_NPC`)\*\*

&nbsp; - \*\*AI Controller (`BP\_AICONTROL\_NPC`)\*\*

&nbsp; - \*\*Blueprint de NPC (`BP\_NPC`)\*\*

\- Implementación de tareas personalizadas:

&nbsp; - Buscar nueva ubicación

&nbsp; - Mover al objetivo



📂 \*\*Ubicación:\*\*  

`Content/jdma/ia/`



---



\## ✨ 3. Sistemas de partículas y efectos visuales



Se integraron cuatro sistemas de partículas con funciones específicas:



| Partícula | Función principal |

|------------|------------------|

| `NS\_LUZ`   | Iluminación ambiental |

| `NS\_AZUL`  | Indicación de zonas con loot o puntos de interés |

| `NS\_PLANTA`| Efecto decorativo natural |

| `NS\_ROJO`  | Señalización de zonas peligrosas |



📂 \*\*Ubicación:\*\*  

`Content/jdma/Particulas/`



---



\## 🧩 4. Modelos y entorno



\- Estructura organizada por tipo de elemento:

&nbsp; - `destruibles/` → objetos rompibles.

&nbsp; - `newguard/` → personaje principal y animaciones.

&nbsp; - `plantitas/`, `balón/`, `estadio/`, etc. → props decorativos y funcionales.

\- Se añadió ambientación general al mapa principal con integración de iluminación y materiales personalizados.



📂 \*\*Ubicación:\*\*  

`Content/jdma/Models/`



---



\## 💾 5. Sistema de inventario y guardado



\- Implementación completa del \*\*Inventario HUD (`WBP\_HUD`)\*\*.

\- Soporte para visualización de íconos de objetos recogibles.

\- Definición de estructuras y enumeraciones para objetos (`StructNEnum`).

\- Sistema de guardado de variables mediante `SG\_SaveGame`.



📂 \*\*Ubicación:\*\*  

`Content/jdma/Maps/Inventario/`  

`Content/jdma/Maps/SaveGame/`



---



\## 🧭 6. Menús e interfaz de usuario



\- \*\*Menú principal (`UW\_MainMenu`)\*\*

\- \*\*Menú de opciones (`UW\_Opciones`)\*\*

\- \*\*Menú de pausa (`UW\_Pausa`)\*\*

\- Uso de una \*\*tipografía personalizada\*\* y fondos visuales.

\- Menú funcional vinculado al mapa `MainMenu`.



📂 \*\*Ubicación:\*\*  

`Content/jdma/Maps/Widgets/`



---



\## 🌍 7. Mapas principales



| Mapa | Descripción |

|------|--------------|

| `LV\_1` | Nivel principal del juego con todos los sistemas integrados. |

| `MainMenu` | Escena inicial que carga el menú principal. |



📂 \*\*Ubicación:\*\*  

`Content/jdma/Maps/`



---



\## 📜 Commits principales



1\. `Implementación de barra de vida, soporte para teclado/gamepad y reemplazo de personaje principal con animaciones.`

2\. `Implementación inicial de IA para NPC (Blackboard, Behavior Tree, AI Controller y tareas personalizadas).`

3\. `Creación de sistemas de partículas (NS\_LUZ, NS\_AZUL, NS\_PLANTA, NS\_ROJO).`

4\. `Organización de modelos y props (destruibles, personaje principal, entorno).`

5\. `Integración de menús, inventario y sistema de guardado.`



---





