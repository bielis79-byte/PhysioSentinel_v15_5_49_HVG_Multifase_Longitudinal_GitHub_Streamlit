# PhysioSentinel v15.5.49 · Panel HVG multifase y longitudinal

## Pestaña 5 · Panel HVG multivariable

El panel deja de estar limitado a la fase seleccionada en el selector superior de
Poincaré/grafos. Se añade un selector independiente con cuatro modos:

1. **Evolución de una fase entre registros**
   - Ejemplo: todos los Basales de diferentes registros.
   - Una columna por registro en orden cronológico.
   - Línea de tendencia longitudinal cuando existen al menos dos registros.

2. **Basal · Ejercicio · Recuperación por registro**
   - Muestra los tres grandes grupos fisiológicos juntos.
   - Basal agrupa Basal/Basal2...
   - Ejercicio agrupa E1–E6.
   - Recuperación agrupa R1–R6.
   - Si existen varias subfases, se usa la media de la métrica HVG del grupo para ese registro.

3. **Fases concretas entre registros**
   - Permite seleccionar, por ejemplo, Basal + E1 + R1.
   - Las fases aparecen como columnas agrupadas por registro y con tendencias longitudinales independientes.

4. **Selección actual de Poincaré/grafos**
   - Conserva el comportamiento previo para compatibilidad.

Se mantienen la selección multivariable, la selección topológica recomendada,
la paginación y la arquitectura de rendimiento para cohortes grandes.

## Versionado histórico

El archivo histórico aportado documentó **169 app.py únicos** hasta la etapa anterior.
Tras generar v15.5.48 y esta v15.5.49, la evidencia acumulada pasa a:

**≥171 iteraciones únicas de desarrollo documentadas.**

## Sin cambios

No se modifica la fisiología de Control Autonómico, IID, predicción,
longitudinal, integrado 70/30, contextualización por edad/sexo, atractores
ni el resto de pestañas.
