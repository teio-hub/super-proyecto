Ahorro Programado

Este proyecto contiene las pruebas unitarias para el cálculo de cuotas de ahorro programado,
usando la fórmula de anualidad ordinaria para determinar el pago regular requerido.

## Contenido

### test_ahorro.py

Implementa las siguientes pruebas unitarias:

Caso Normal 1
- Entradas
  - Meta: 10.000.000
  - Tasa: 1% mensual
  - Plazo: 24 meses
- Salidas
  - Cuota: 370.734.72

Caso Normal 2
- Entradas
  - Meta: 5.000.000
  - Tasa: 0.75% mensual
  - Plazo: 12 meses
- Salidas
  - Cuota: 399.757.38

Caso Normal 3
- Entradas
  - Meta: 20.000.000
  - Tasa: 0.83% mensual
  - Plazo: 36 meses
- Salidas
  - Cuota: 478.968.21

Tasa Cero
- Entradas
  - Meta: 10.000.000
  - Tasa: 0% mensual
  - Plazo: 24 meses
- Salidas
  - Cuota: 416.666.67

Plazo 1 Mes
- Entradas
  - Meta: 500.000
  - Tasa: 1% mensual
  - Plazo: 1 mes
- Salidas
  - Cuota: 500.000

Abono Extra
- Entradas
  - Meta: 10.000.000
  - Tasa: 1% mensual
  - Plazo: 24 meses
  - Abono: 2.000.000
  - Mes del abono: 24
- Salidas
  - Cuota: 296.587.78

Cuota Única
- Entradas
  - Meta: 20.000.000
  - Tasa: 0.83% mensual
  - Plazo: 36 meses
  - Abono: 5.000.000
  - Mes del abono: 36
- Salidas
  - Cuota: 359.226.16

Error Meta Cero
- Entradas
  - Meta: 0
  - Tasa: 1% mensual
  - Plazo: 24 meses
- Salidas
  - Error: La meta debe ser mayor que cero

Error Plazo Cero
- Entradas
  - Meta: 10.000.000
  - Tasa: 1% mensual
  - Plazo: 0
- Salidas
  - Error: El plazo debe ser al menos 1 mes

Error Tasa Negativa
- Entradas
  - Meta: 10.000.000
  - Tasa: -2% mensual
  - Plazo: 24 meses
- Salidas
  - Error: La tasa de interés no puede ser negativa

Error Plazo Negativo
- Entradas
  - Meta: 20.000.000
  - Tasa: 1% mensual
  - Plazo: -12 meses
- Salidas
  - Error: El plazo no puede ser negativo

### logica_ahorro.py

Implementa la funcionalidad que cumple con estos casos.