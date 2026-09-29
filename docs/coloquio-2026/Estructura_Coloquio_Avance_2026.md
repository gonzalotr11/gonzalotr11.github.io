# Coloquio de avance doctoral — Estructura propuesta (v2)

*Gonzalo Torres Rosales · 26-09-2026 · 15 min · español · HTML publicado en GitHub*
*Base: candidatura (ene-2026), comentarios de comisión (mar-2026), reformulación (ago-2026), carpetas Article1, Article2 y Art3*

**Hilo narrativo (una frase):** *la candidatura proponía reconstruir la riqueza para estudiar la seguridad económica. Al implementarla aprendimos que la imputación no sostiene inferencias sustantivas, y la tesis se reorienta hacia la **inseguridad económica**, leída desde posiciones económicas complejas (ingreso, activos, ocupación/formalidad y trayectoria) y sus huellas en el desarrollo infantil (A1), en las trayectorias educativas (A2) y en las trayectorias financieras del hogar (A3).*

**Presupuesto: 16 láminas en ~15 min.** Tesis ≈ 4 min · A1 ≈ 6 min · A2 ≈ 3 min · A3 ≈ 1,5 min · cierre ≈ 0,5 min.

---

## I. La tesis (4 láminas · ~4 min)

**0. Portada.** Título actualizado, por definir. Tentativo: *Inseguridad económica y desigualdad: posiciones económicas de los hogares y trayectorias de desarrollo en Chile.*

**1. De la candidatura a hoy.** Una sola lámina en dos columnas, *antes | ahora*:
- **Antes (enero de 2026):** la riqueza como infraestructura de seguridad; imputación ML (EFH→CASEN→ADMIN) como base de los artículos 2 y 3.
- **Advertencias de la comisión:** detalle de portafolio no alcanzable, endogeneidad del proxy y riqueza reducida a un escalar (Pfeffer y segundo evaluador).
- **Lo que mostró la implementación:** al propagar la incertidumbre (100 imputaciones), el efecto *naive* era hasta ~90× mayor y con signo invertido; con la incertidumbre propagada el resultado es nulo pero robusto. **Se abandona la imputación como eje.**
- Mensaje oral: *la evidencia confirmó lo que la comisión anticipó, y eso ordenó el giro.*

**2. La pregunta reformulada.** *¿Cómo se relaciona la posición económica compleja de los hogares con la inseguridad económica, y cómo esta se traduce en desigualdades de desarrollo infantil y educativo?* La inseguridad se lee en tres momentos: **exposición** al shock (antes), **amortiguación** (durante) y **recomposición** (después). La posición económica se entiende como multidimensional: ingreso, activos, ocupación/formalidad y su trayectoria en el tiempo.

**3. Mapa de la tesis.** Tabla:

| | A1 | A2 | A3 |
|---|---|---|---|
| Escala | Hogar en el tiempo | Hogar ↔ escuela | Estructura financiera del hogar |
| Datos | ELPI 2010–2024 | MINEDUC/CEM + SIMCE | Panel EFH |
| Posición económica | Trayectoria ocupacional, shocks de ingreso, activos | Movilidad de dependencia como hecho económico | Configuraciones de activos y deudas |
| Outcome | Desarrollo cognitivo y socioemocional | Expectativas y trayectoria educativa | Trayectorias de (in)seguridad financiera |
| Estado | Análisis completo, redacción | Diseño | Idea y diseño inicial |

## II. Artículo 1 — Trayectorias económicas del hogar y desarrollo infantil (6 láminas · ~6 min)

**4. Pregunta, datos y antesala.** No se pregunta *si* la privación daña, sino cómo **momento, duración y reversibilidad** moldean su costo. ELPI tiene 4 olas y más de 15.000 niños. *Antesala* (en un recuadro lateral): los activos no amortiguan el daño directo (H1 ✗), pero reducen la incidencia de shocks (OR 0,53–0,85) y facilitan la recuperación (H2 y H3 ✓). El empleo decide la recuperación (22–30 % frente a 48–71 %). Esto motiva mirar **trayectorias**, no eventos.

**5. Diseño.** Diagrama de la tipología 2×2 (estado ocupacional en 2012 × estado en 2017): estabilidad, recuperación, deterioro y cronicidad. Identificación con **línea base propia**: TVIP 2017 controlando por TVIP 2012, con exposición estrictamente posterior a la línea base. N = 6.809.

**6. Resultado central.** Gráfico de coeficientes con IC 95 %: recuperación −0,11 DE ≈ cronicidad −0,13 DE; deterioro +0,04 (n.s.); activos 2012 +0,13 DE. Frase de cierre: ***la recuperación económica no revierte el costo ya incurrido.***

**7. Mecanismos.** El estrés parental (PSI) media el 12–17 % del efecto de los activos sobre el TVIP y el 62–74 % sobre el CBCL. Lectura: la inversión opera sobre lo cognitivo y el estrés sobre lo socioemocional; son canales de dominios distintos que no compiten entre sí.

**8. Robustez y horizonte largo.** Mini tabla:
- Estructura familiar: el efecto principal no cambia; la inestabilidad de cuidadores tiene un costo propio.
- Ganancia simétrica (M5) y shock regional (M6): sin cambios.
- Horizonte 2012→2024: la cronicidad persiste (−0,085) y la penalización por recuperación se atenúa, lo que muestra que los activos importan más a largo plazo.

**9. Límites y estado.** Límites declarados: selección tipo Mayer, atenuación en la variable dependiente rezagada y mediadores contemporáneos. Estado: introducción, marco y métodos redactados, análisis completo, faltan resultados y discusión. Revista objetivo: *World Development*. Ponencia en DEMOSAL (marzo de 2027).

## III. Artículo 2 — Movilidad escolar como hecho económico, redes y expectativas (3 láminas · ~3 min)

**10. Encuadre: el cambio de colegio como hecho económico.** En Chile, moverse entre dependencias (municipal, particular subvencionado con copago, particular pagado) es una **decisión económica del hogar**. Subir compromete recursos bajo incertidumbre y bajar puede señalar un shock. La movilidad escolar es así una forma observable de la (in)seguridad económica en datos administrativos. Esa movilidad reconfigura además la **red de pares** del estudiante (DiMaggio & Garip 2012), y a través de ella sus expectativas.
- *Por construir:* un proxy de la condición económica del hogar en los datos administrativos. Candidatos: la trayectoria de la condición de alumno prioritario/preferente (SEP), el arancel o copago del colegio de destino y el índice de elitización. **Hay que verificar la disponibilidad.**

**11. Diseño.** Δ = expectativa del estudiante (II medio) − expectativa de los padres (4° básico). Es una línea base pre-movilidad con otro informante. Se consideran movilizados quienes cambian entre ambas mediciones, con dos grupos de referencia (excompañeros de origen y nuevos compañeros). Pruebas previstas:
  - (a) dirección del movimiento (ascenso o descenso) como hecho económico;
  - (b) formas funcionales de exposición a pares (continua, umbral, densidad);
  - (c) divergencia de varianza (réplica de DiMaggio & Garip 2011).

**12. Contribución y estado.** Se atacan a la vez la selección (vía Δ) y la desigualdad (vía varianza). El antecedente más cercano es Cattan, Salvanes & Tominey (2022). El piloto de 2023 tuvo 205.886 cuestionarios con 100 % de match. Hay un Plan A (expectativas) y un Plan B (rendimiento y selección en educación superior), con una regla de cobertura de ≥60–70 %. Siguiente paso: diagnóstico de completitud del Cuestionario SIMCE.

## IV. Artículo 3 — Redes de activos y deudas (2 láminas · ~1,5 min)

**13. Idea.** La seguridad económica como **propiedad relacional**. Los nodos son instrumentos financieros (ahorro, hipoteca, consumo bancario o de retail, deuda educativa, mora) y los hogares son trayectorias que los recorren. Se distinguen "puentes seguros" de "espirales de estrés". Referencia: Cheng & Park (2020), para quienes las fronteras de movilidad equivalen a fronteras de clase.

**14. Diseño y estado.** Panel EFH (llave de panel entre olas). Proyección bipartita, comunidades por flujos e índice de seguridad. Respuesta a Pfeffer: el índice se compara con componentes simples en capacidad predictiva. Estado: argumento escrito y panel procesado. Falta actualizar el encuadre, que aún se apoya en las medidas imputadas del antiguo Art. 1.

## V. Cierre (1 lámina · ~0,5 min)

**15. Síntesis, próximos pasos y preguntas a la comisión.** Tres escalas de la inseguridad económica: el hogar en el tiempo, el hogar frente a la escuela y la estructura financiera. Cronograma breve. Dos o tres preguntas concretas para la comisión.

**Anexo (no se expone, sirve para preguntas).** Tabla completa *comentario de comisión → respuesta*; detalle del fracaso de la imputación; tablas M0–M6 del A1; mecanismos de DiMaggio & Garip.

---

## Pendientes para las próximas sesiones
- Título de tesis y pregunta general definitivos.
- A2: confirmar qué proxy económico del hogar existe en los datos MINEDUC (prioritario/preferente, copago) y redactar la hipótesis sobre el ascenso y el descenso.
- A3: nombre del índice (IPPS o SCI) y reemplazar "patrimonial" por *wealth/financial* en la versión en inglés.
- Figuras: gráfico de coeficientes del A1 (datos de la Tabla 1 de DEMOSAL) y diagrama de la tipología 2×2.
- Cronograma hasta la defensa.
