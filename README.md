# Eficacia-de-la-Se-al-de-Reversi-n-Sectorial
Eficacia de la Señal de Reversión Sectorial

Eficacia de la Señal de Reversión Sectorial
¿Dónde Funciona Mejor el RSI < 30?

Este proyecto implementa una consulta SQL que evalúa qué tan efectiva es una señal clásica de reversión (RSI < 30) en distintos sectores, midiendo el rendimiento promedio a 10 días posterior a la señal.

La idea no es preguntar si la señal funciona, sino dónde funciona mejor.

🧠 Idea central

La sobreventa no se comporta igual en todos los sectores.

Algunos sectores:

rebotan rápido

absorben bien el pánico

muestran reversión técnica limpia

Otros:

siguen cayendo

reflejan problemas estructurales

El contexto sectorial define la eficacia de la señal.

🎯 Valor de negocio

Optimiza estrategias de reversión

Útil para:

asignación de capital

filtros sectoriales

mejora de expectancy

Convierte señales genéricas en señales contextuales

🗄️ Estructura de datos esperada
tickers
campo	descripción
ticker_id	Identificador del activo
sector	Sector económico
indicadores_tecnicos
campo	descripción
ticker_id	Identificador
fecha	Fecha
rsi_14	RSI de 14 períodos
precios_diarios
campo	descripción
ticker_id	Identificador
fecha	Fecha
close	Precio de cierre
⚙️ Lógica de la consulta

Detecta señales de sobreventa (RSI < 30)

Obtiene el precio de cierre del día de la señal

Calcula el precio 10 días después

Mide el rendimiento porcentual post-señal

Agrega resultados por sector

🔎 Interpretación de resultados

Rendimiento alto → sector ideal para reversión

Rendimiento bajo o negativo → sobreventa estructural

Permite:

priorizar sectores

evitar señales de baja calidad

🚀 Posibles extensiones

Analizar múltiples horizontes (5, 20 días)

Medir drawdown máximo post-señal

Ajustar por volatilidad sectorial

Comparar con otras señales (ADX, SMA)

📝 Notas finales

No es una estrategia completa

Es un motor de validación contextual

Clave para mejorar sistemas existentes
