---
video_id: _5X-_kuklvU
title: "5 Patrones de Diseño que Todo Dev Debería Dominar"
model: gpt-oss:20b
date: 2025-08-19T00:08:05.332635
---

[END]

### 📌 Detalles Técnicos (en Español)

- **Mediator (Patrón Conductual)**: Centraliza la comunicación entre objetos, reduciendo acoplamientos directos.  
- **Observer (Patrón Conductual)**: Mantiene una lista de suscriptores que reciben notificaciones cuando el estado del objeto cambia.  
- **Eventos**: Mecanismo de disparo y escucha en C#.  
- **PropertyChanged**: Notificación de cambio de propiedad, típica en MVVM/WPF.  
- **Microservicios**: Arquitectura distribuida donde los patrones ayudan a gestionar la complejidad.  

### 📚 Clasificación

- **Profundidad**: Intermedio‑Avanzado  
- **Tema**: Patrones de diseño (conductuales) y su aplicación en arquitecturas modernas.  

---

## 🔍 Patrones Ocultos
1. **Patrón principal:** **Mediator** – centraliza la comunicación entre componentes para evitar acoplamientos directos.  
2. **Patrón secundario:** **Observer** – notifica automáticamente a suscriptores cuando el estado de un objeto cambia.  
3. **Patrón emergente:** **Eventos en C#** – mecanismo subyacente que permite la implementación de Observer y facilita la comunicación asíncrona entre objetos.

## 🌐 Conexiones Profundas
- **Causa raíz:** La necesidad de gestionar la complejidad creciente en sistemas distribuidos (microservicios) y UI reactivas.  
- **Efectos sistémicos:**  
  - *Mediator* reduce la dependencia directa entre componentes, pero introduce un punto único de fallo si el Mediator falla.  
  - *Observer* permite extensibilidad sin modificar el objeto observador, pero puede generar cascadas de notificaciones si no se controla la suscripción.  
- **Interdependencias críticas:**  
  - En microservicios, *Mediator* se usa como bus de mensajes interno; su rendimiento afecta la latencia global.  
  - En MVVM/WPF, *Observer* (PropertyChanged) es esencial para la sincronización de UI y modelo.

## 🚀 Disrupciones Detectadas
- **Cambio de paradigma:** De un enfoque acoplado a uno desacoplado mediante mediadores y observadores.  
- **Oportunidad emergente:** Implementar *Mediator* como bus de eventos propio (ej. MediatR en .NET) para un desarrollo más limpio y testeable.  
- **Amenaza sistémica:** El acoplamiento implícito que el Mediator puede generar si se sobreutiliza o se expone públicamente a demasiados componentes.

## ⚡ Dinámicas Subyacentes
- **Poder real:** El *Mediator* controla la comunicación; su diseño determina la flexibilidad y la facilidad de mantenimiento.  
- **Influencias ocultas:** La cultura de “micro‑servicios” impulsa el uso de Mediator como bus interno; la experiencia previa con eventos en C# fomenta Observer.  
- **Motivaciones no declar