<h1>📌 Calculadora de Ahorro Programado 
  <img src="https://media.giphy.com/media/13HgwGsXF0aiGY/giphy.gif" width="60px">
</h1>

---

###  Creadores

- María Paula Ospina Zabala
- Alejandro Tello Giraldo
  
 --- 
 ### 👩‍💻 Persona entrevistada
- **Nombre:** Karen Londoño 
- **Cargo:** Gerente de proyectos en una compañía financiera
- **Experiencia relacionada:** Finanzas
- **Fecha de la entrevista:** 08/02/2026

---

### 📖 Descripción del Proyecto

La **Calculadora de Ahorro Programado** es una aplicación diseñada para ayudar a las personas a planificar su ahorro mensual con el fin de alcanzar una meta financiera específica en un periodo de tiempo determinado.

La aplicación permite calcular el valor que se debe ahorrar mensualmente y, además, ofrece la posibilidad de registrar **abonos extra** en cualquier momento y por cualquier cantidad, ajustando el ahorro restante de forma automática.

---

### 🎯 Objetivo

Esta herramienta busca facilitar al usuario una ayuda para alcanzar su meta de ahorro de una manera sencilla, además de brindarle una planificación financiera personal que permita:

-  Definir una meta de ahorro.
-  Establecer un plazo en meses.
-  Calcular el ahorro mensual necesario.
-  Registrar abonos adicionales.
-  Visualizar el progreso del ahorro.

## 📥 Entradas del Sistema

El usuario debe ingresar:

- **Meta de ahorro (Meta)**  
- **Tasa de interés mensual (i)**  
- **Plazo en meses (n)**  
- **Abonos extra (opcional)**
- **Valor del abono**

 ## ⚙️ Proceso del Sistema
La aplicación utiliza la fórmula financiera de ahorro programado:

**Cuota = Meta × [ i / ((1 + i)^n − 1) ]**

Donde:
- **Meta** = Valor objetivo a alcanzar  
- **i** = Tasa de interés mensual  
- **n** = Número de meses  
- **Cuota** = Valor que debe ahorrarse mensualmente  

❗ **Caso especial:** Si la tasa es 0%, se usa: **Cuota = Meta / n** ❗

### Funcionamiento:
1. **Validación:** Se verifican que meta, plazo y tasa sean válidos.
2. **Cálculo inicial:** Se determina la cuota mensual con base en la fórmula.
3. **Simulación mes a mes:** Se proyecta el crecimiento del ahorro aplicando los intereses.
4. **Abonos extras (opcional):**
   - Se suman al capital acumulado en el mes indicado.
   - Empiezan a generar intereses inmediatamente.
   - Se recalcula la cuota para los meses restantes.
5. **Resultado final:** Se muestra la cuota mensual, total de intereses y total ahorrado.

---
## 📤 Salidas del Sistema
El sistema mostrará:
-  **Cuota mensual:** Valor que debe ahorrarse cada mes para alcanzar la meta.
-  **Total de intereses:** Dinero adicional generado durante el periodo de ahorro.
-  **Total ahorrado:** Suma de la meta más los intereses ganados.
-  **Nuevo plan tras abonos:** Si se realizan abonos extras, muestra la cuota recalculada.
-  **Confirmación de meta:** Mensaje cuando la meta sea alcanzada.

### Mensajes de Error
En caso de datos inválidos:
- ❌ "ERROR: La meta debe ser mayor que cero"
- ❌ "ERROR: El plazo debe ser al menos 1 mes"
- ❌ "ERROR: La tasa de interés no puede ser negativa"
- ❌ "ERROR: El plazo no puede ser negativo"

---

