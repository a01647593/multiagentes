# multiagentes - Sistema Multiagente para Gestión de AGV

## Descripción del proyecto

Este proyecto desarrolla una simulación de un almacén logístico utilizando un Sistema Multiagente (SMA). El objetivo es representar el comportamiento de varios vehículos AGV que reciben misiones de transporte, se comunican, negocian entre ellos y se desplazan dentro del almacén evitando conflictos de ruta.

La simulación utiliza 6 agentes AGV, todos representados mediante el modelo `V4_Apilador_Stacker`.

El sistema integra el entorno desarrollado previamente, las misiones de transporte, el movimiento de los agentes, niveles de batería, negociación de misiones, planificación de rutas y métricas de desempeño.

Además, se compara una estrategia base o baseline contra una estrategia inteligente basada en una heurística de utilidad.

---

## Integrantes

- Integrante 1: Desiderio Ortegon Morton
- Integrante 2: Luis Tonchez
- Integrante 3: Sebastian Martinez
- Integrante 4: Julian Bustos
- Integrante 5: Ayhan Ben Halima


---

## Objetivo

El objetivo principal es mejorar la asignación de misiones entre los AGV para reducir recorridos innecesarios, evitar congestión y utilizar de mejor manera los recursos disponibles.

El sistema busca responder la siguiente pregunta:

**¿La estrategia inteligente propuesta mejora el desempeño del Sistema Multiagente en comparación con una estrategia base?**

---

## Arquitectura del sistema

La arquitectura general del proyecto es:

```text
Entorno
   ↓
Mission Manager
   ↓
Publicación de misión
   ↓
Agentes AGV
   ↓
Negociación / Subasta
   ↓
Selección del agente
   ↓
Planificación de ruta
   ↓
Movimiento
   ↓
Pickup
   ↓
Dropoff
   ↓
Actualización de métricas
