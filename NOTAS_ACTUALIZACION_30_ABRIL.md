# Actualización del informe Barbacoaj 2026: 30 de abril

**Fecha de edición:** 25 de noviembre de 2026.

## Qué motivó el cambio

Ariel Brukman, integrante presente en el encuentro del 30/04/2026, informó que asistieron solo tres integrantes y prácticamente no hubo ejecución musical sostenida. Durante parte del encuentro escucharon versiones grabadas de canciones propias generadas con Suno, que no ingresaban normalmente a la mezcla auxiliar utilizada por OBS, y no hablaron por los micrófonos.

La versión anterior del informe clasificaba como música el **78,04 %** de los **63 minutos analizables** de la transmisión. Esa clasificación queda invalidada por evidencia contextual. El detector marcaba los primeros 40 minutos completos como música a pesar de una señal notablemente estable y con muy poca variación espectral.

## Cómo se representó

- El 30/04 se cuenta, a efectos de los indicadores, como fecha **sin ejecución musical sostenida documentada por testimonio**: 0 min de ejecución sostenida y 63 min sin ejecución sostenida, conservando 0,5 min de falta de señal.
- **No** se afirma que se haya hablado durante esos 63 minutos: también hubo convivencia, bebida y escucha de música reproducida.
- La atribución no deriva de una escucha humana cronometrada minuto a minuto; pudieron existir notas ocasionales. Es una decisión metodológica explícita sobre la **categoría de ejecución sostenida**.
- En el HTML, esta fecha aparece con el símbolo † y un aviso. Los mapas y el «jueves promedio» están recalculados con esta corrección.

## Impacto numérico

| Indicador | Antes | Después |
|---|---:|---:|
| Ejecución musical estimada, año | 54,95 % | **53,43 %** |
| Tiempo sin ejecución sostenida, año | 45,05 % | **46,57 %** |
| Ejecución musical estimada, abril | 61,62 % | **48,12 %** |
| Ejecución musical atribuida al 30/04 | 49,17 min | **0 min (criterio contextual)** |

El denominador anual sigue siendo de **3236,3 minutos analizables** y el universo comprende **34 jueves de ensayo / 37 emisiones**. La transmisión técnica del lunes 7/09, de 42 segundos, se conserva en el índice de fuentes, pero no entra en el cálculo.

Si el 30/04 hubiera contenido cinco minutos de ejecución sostenida, el indicador anual sería aproximadamente **53,58 %**. Ese valor es un escenario hipotético, no una nueva medición.

## Cambios aplicados

- `index.html`: indicadores, texto, mapas de calor por fecha, mapa del jueves promedio, resultados mensuales, tabla, ficha del 30/4, sección metodológica y enlaces a datos.
- `informe.pdf`: indicadores, figuras, tabla del 30/4, análisis del 5/3 con nuevo punto de partida, metodología y una nueva página para el caso del 30/4.
- `resultados_por_ensayo_2026.csv`, `resultados_mensuales_2026.csv`, `mapa_calor_minuto_2026.csv`: tablas revisadas con indicación de procedencia de la corrección.
- `correccion_documentada_30_abril_2026.csv`: registro específico de evidencia y decisiones.
- `diagnostico_por_tramos_30_abril.csv`: señales que explican el falso positivo del sistema.
- `jueves_promedio_2026_5min.csv`: distribución media recalculada por hora real de Buenos Aires.
- `revision_05_marzo_etiquetas.csv` e `indice_emisiones_2026.csv`: copias de los archivos de respaldo existentes, sin cambios.

No se reentrenó el modelo ni se escucharon manualmente todas las emisiones de 2026. Otras discrepancias pueden detectarse cuando integrantes de la banda revisen sus recuerdos y las grabaciones.
