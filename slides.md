---
title: 🔌 MCP Server vs 🧠 Function Calling
subtitle: Patrones Complementarios en Sistemas de IA
author: Germán Aliprandi
date: Abril 2025

theme: geist
colorSchema: light
canvasWidth: 1280
transition: fade

defaults:
  layout: cover
  transition: fade

seoMeta:
  title: "MCP Server vs Function Calling: Separación Clara de Responsabilidades en Arquitecturas de IA"
  description: "Descubre por qué el MCP Server debe ser un puerto de I/O y cómo la Function Calling ejecuta lógica inteligente. Caso práctico en retail para exponer productos, precios y recomendaciones."
  keywords: "MCP Server, Function Calling, arquitectura IA, sistemas inteligentes, API design, inteligencia artificial, patrones de diseño, Cencosud Tech"
  ogTitle: "MCP Server vs Function Calling: La Separación Correcta de Responsabilidades en Arquitecturas de IA"
  ogDescription: "¿Debería tu MCP Server ejecutar lógica de negocio? Descubre el patrón correcto con un caso práctico de retail para exponer productos, precios y recomendaciones inteligentes."
  ogUrl: "https://galiprandi.github.io/mcp-vs-fnc"

  twitterCard: "summary_large_image"
  twitterCreator: "@galiprandi"
  canonicalUrl: "https://galiprandi.github.io/mcp-vs-fnc"
---

# {{ $frontmatter.title }} 
### {{ $frontmatter.subtitle }}

**Caso de uso:** Exponer productos, precios y recomendaciones inteligentes a clientes externos

<div class="mt-10 text-l">
<b>{{ $frontmatter.author }}</b><br>
{{ $frontmatter.date }}
</div>

<div class="absolute bottom-8 right-8 text-l bg-black/10 px-4 py-2 rounded-full">
  ➡️ Navega con la flecha derecha del teclado
</div>

---
theme: geist
layout: default
---

# 🛒 Caso de Uso: Retail Inteligente

## Un cliente externo (ChatGPT, n8n, partner) pregunta:

#### "¿Cuál es el precio del Shampoo Elvive Reparación Total 5, 750ml?  
#### ¿Qué productos relacionados en oferta me recomiendan?"

<div class="grid grid-cols-2 gap-4 mt-8">
  <div class="bg-blue-50 p-4 rounded-lg border border-blue-200">
    <h3 class="text-xl font-bold mb-2">🔍 Consulta Completa</h3>
    <ul class="list-disc pl-5">
      <li>Precio específico de un producto</li>
      <li>Recomendaciones inteligentes</li>
      <li>Información sobre ofertas vigentes</li>
    </ul>
  </div>
  <div class="bg-blue-50 p-4 rounded-lg border border-blue-200">
    <h3 class="text-xl font-bold mb-2">⚙️ Necesidades Técnicas</h3>
    <ul class="list-disc pl-5">
      <li>Datos en tiempo real</li>
      <li>Inteligencia contextual</li>
      <li>Respuesta estandarizada</li>
    </ul>
  </div>
</div>

---
theme: geist
colorSchema: light
layout: default
---

# ❓ ¿Dónde vive la inteligencia?

## Piensa por un momento...

<div class="text-3xl mt-12">
¿Dónde pondrías la lógica de recomendación: 
<br>
<b>dentro del MCP Server</b> o <b>en una función externa</b>?
</div>

<div class="mt-12 grid grid-cols-2 gap-4">
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200 text-center">
    <div class="text-5xl mb-4">🔌</div>
    <div class="text-xl">MCP Server</div>
  </div>
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200 text-center">
    <div class="text-5xl mb-4">🧠</div>
    <div class="text-xl">Function Calling</div>
  </div>
</div>

---
theme: geist
colorSchema: light
layout: default
---

# ❓ ¿Dónde vive la inteligencia?

## La respuesta definitiva

<div class="grid grid-cols-2 gap-8 mt-8">
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200">
    <div class="text-2xl font-bold mb-4 flex items-center">
      <span class="mr-2">🔌</span> MCP Server = PUERTO DE CONEXIÓN
    </div>
    <ul class="list-disc pl-6 space-y-2 text-lg">
      <li>Solo permite la comunicación <span class="ml-1">🔄</span></li>
      <li>No ejecuta lógica <span class="ml-1">💡</span></li>
      <li>Estándar universal (como USB) <span class="ml-1">🌐</span></li>
      <li>"¿Qué necesitas?" <span class="ml-1">🤔</span></li>
    </ul>
  </div>
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200">
    <div class="text-2xl font-bold mb-4 flex items-center">
      <span class="mr-2">🧠</span> Function Calling = CEREBRO INTELIGENTE
    </div>
    <ul class="list-disc pl-6 space-y-2 text-lg">
      <li>Ejecuta lógica compleja <span class="ml-1">🧮</span></li>
      <li>Toma decisiones <span class="ml-1">🎯</span></li>
      <li>Contiene conocimiento especializado <span class="ml-1">📚</span></li>
      <li>"Esto es lo que necesitas" <span class="ml-1">✅</span></li>
    </ul>
  </div>
</div>

<div class="mt-12 text-2xl bg-yellow-50 p-4 rounded-lg border border-yellow-200">
  <b>✅ DIFERENCIA CLAVE:</b> 
  <div class="mt-2">
    El MCP pregunta, la Function responde.<br>
    El MCP conecta, la Function piensa.<br>
    El MCP es un adaptador, la Function es un ejecutor.
  </div>
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🤔 ¿Dónde trazar el límite?

## Piensa en tu propio sistema...

<div class="text-3xl mt-12">
¿Cómo decidirías qué va en el MCP<br>
y qué pertenece a la Function Calling?
</div>

<div class="mt-10 text-2xl text-center">
<b>Considera:</b>
<br>
• ¿Quién controla el código?<br>
• ¿Dónde vive la lógica de negocio?<br>
• ¿Cómo manejas los errores?
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🔌 MCP Server vs 🧠 Function Calling

<div class="grid grid-cols-2 gap-8 mt-8">
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-blue-700">
      <span class="mr-2">🔌</span> MCP Server
    </div>
    <div class="text-xl mb-4">📍 <b>Ubicación:</b> Capa de exposición</div>
    <div class="text-xl mb-4">⚡ <b>Ejecución:</b> Liviana, orquestación</div>
    <div class="text-xl mb-4">🔐 <b>Control:</b> Parcial</div>
    <div class="text-xl mb-4">📈 <b>Escalabilidad:</b> Alta (peticiones simples)</div>
    <div class="text-xl">🎯 <b>Responsabilidad:</b> Contrato, formato, seguridad</div>
  </div>
  <div class="bg-purple-50 p-6 rounded-lg border border-purple-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-purple-700">
      <span class="mr-2">🧠</span> Function Calling
    </div>
    <div class="text-xl mb-4">📍 <b>Ubicación:</b> Microservicio interno</div>
    <div class="text-xl mb-4">⚡ <b>Ejecución:</b> Pesada, con lógica</div>
    <div class="text-xl mb-4">🔐 <b>Control:</b> Total</div>
    <div class="text-xl mb-4">📈 <b>Escalabilidad:</b> Variable (modelo, carga)</div>
    <div class="text-xl">🎯 <b>Responsabilidad:</b> Decisión, recomendación, cálculo</div>
  </div>
</div>

<div class="mt-10 text-3xl text-center bg-yellow-50 p-6 rounded-lg border border-yellow-200">
  <b>💡 Regla de oro:</b><br>
  "El MCP pregunta. La función piensa."
</div>

---
theme: geist
colorSchema: light
layout: default
---

# ⚠️ ¿Por qué no hacerlo todo en el MCP?

## Imagina esta situación...

<div class="text-3xl mt-12">
Si pudieras, ¿pondrías toda la lógica<br>
directamente en el MCP Server?
</div>

<div class="mt-10 text-2xl text-center">
<b>Considera estos escenarios:</b>
<br>
• ¿Qué pasa si necesitas cambiar el modelo de recomendación?<br>
• ¿Cómo manejas la seguridad de tu lógica de negocio?<br>
• ¿Cómo pruebas y monitoreas la inteligencia?
</div>

---
theme: geist
colorSchema: light
layout: default
---

# ⚠️ Los peligros de sobrecargar el MCP

<div class="grid grid-cols-2 gap-8 mt-8">
  <div class="bg-red-50 p-6 rounded-lg border border-red-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-red-700">
      <span class="mr-2">❌</span> Pérdida de encapsulamiento
    </div>
    <ul class="list-disc pl-6 space-y-2 text-lg">
      <li>Expones tu arquitectura interna</li>
      <li>Clientes externos dependen de tu implementación</li>
      <li>Cambios internos rompen contratos externos</li>
    </ul>
  </div>
  <div class="bg-red-50 p-6 rounded-lg border border-red-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-red-700">
      <span class="mr-2">❌</span> Dificultad de evolución
    </div>
    <ul class="list-disc pl-6 space-y-2 text-lg">
      <li>No puedes mejorar tu modelo sin romper integraciones</li>
      <li>Testing más complejo y menos aislado</li>
      <li>Monitoreo entrelazado entre capas</li>
    </ul>
  </div>
</div>

<div class="mt-10 grid grid-cols-2 gap-4">
  <div class="bg-yellow-50 p-6 rounded-lg border border-yellow-200">
    <div class="text-2xl font-bold mb-2">🛡️ Lección clave</div>
    <div class="text-xl">
      <b>El MCP debe ser un cascarón vacío:</b><br>
      Solo orquestación, sin inteligencia
    </div>
  </div>
  <div class="bg-green-50 p-6 rounded-lg border border-green-200">
    <div class="text-2xl font-bold mb-2">✅ Solución</div>
    <div class="text-xl">
      <b>Capas bien definidas:</b><br>
      MCP = contrato<br>
      Funciones = lógica
    </div>
  </div>
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🌐 ¿Por qué necesitamos el MCP?

## Imagina un escenario sin MCP...

<div class="text-3xl mt-12">
Si las funciones inteligentes son tan poderosas,<br>
¿por qué no permitir que los clientes externos<br>
llamen directamente a nuestras funciones?
</div>

<div class="mt-10 text-2xl text-center">
<b>Considera:</b>
<br>
• ¿Qué tan seguro es exponer directamente tu lógica de negocio?<br>
• ¿Cómo manejarías diferentes versiones de tus funciones?<br>
• ¿Cómo garantizarías un contrato estable para tus clientes?
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🌐 El MCP: Tu Capa Esencial de Abstracción

<div class="grid grid-cols-2 gap-8 mt-8">
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-blue-700">
      <span class="mr-2">❌</span> Sin MCP (Riesgo Alto)
    </div>
    <ul class="list-disc pl-6 space-y-2 text-lg">
      <li>Exposición directa de tu arquitectura interna</li>
      <li>Dependencia de clientes en implementación específica</li>
      <li>Dificultad para versionar y evolucionar</li>
      <li>Sin control centralizado de seguridad</li>
      <li>Formatos de respuesta inconsistentes</li>
    </ul>
  </div>
  <div class="bg-green-50 p-6 rounded-lg border border-green-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-green-700">
      <span class="mr-2">✅</span> Con MCP (Seguridad y Estabilidad)
    </div>
    <ul class="list-disc pl-6 space-y-2 text-lg">
      <li>Contrato estable independiente de la implementación</li>
      <li>Encapsulamiento de la arquitectura interna</li>
      <li>Control centralizado de versiones</li>
      <li>Capa de seguridad y validación unificada</li>
      <li>Formato de respuesta estandarizado</li>
    </ul>
  </div>
</div>

<div class="mt-10 text-3xl text-center bg-yellow-50 p-6 rounded-lg border border-yellow-200">
  <b>💡 Patrón Comprobado:</b><br>
  "El MCP es tu interfaz pública, las funciones son tu implementación privada"
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🛡️ Diseño Robusto: ¿Cómo Implementarlo?

## Piensa en tu implementación...

<div class="text-3xl mt-12">
¿Cómo diseñarías un sistema<br>
que funcione incluso cuando<br>
algunas partes fallen?
</div>

<div class="mt-10 text-2xl text-center">
<b>Considera estos aspectos:</b>
<br>
• ¿Cómo manejas los tiempos de espera?<br>
• ¿Qué haces cuando una función falla?<br>
• ¿Cómo versionas cambios sin romper integraciones?
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🛡️ Diseño Robusto: Separación de Responsabilidades

<div class="grid grid-cols-2 gap-8 mt-8">
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-blue-700">
      <span class="mr-2">🔌</span> MCP Server - Buenas Prácticas
    </div>
    <ul class="list-disc pl-6 space-y-2 text-lg">
      <li>Contrato claro con OpenAPI + JSON Schema</li>
      <li>Validación solo sintáctica (formato del ID)</li>
      <li>Timeout estricto en invocaciones (ej: 800ms)</li>
      <li>Campos opcionales marcados explícitamente</li>
      <li>Versionado independiente del backend</li>
    </ul>
  </div>
  <div class="bg-green-50 p-6 rounded-lg border border-green-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-green-700">
      <span class="mr-2">🧠</span> Function Calling - Buenas Prácticas
    </div>
    <ul class="list-disc pl-6 space-y-2 text-lg">
      <li>SLA definido y monitoreado</li>
      <li>Mecanismos de retry y circuit breaker</li>
      <li>Cache para operaciones costosas</li>
      <li>Modelos ligeros para cumplir tiempos</li>
      <li>Testing aislado de la lógica de negocio</li>
    </ul>
  </div>
</div>

<div class="mt-10 text-3xl text-center bg-yellow-50 p-6 rounded-lg border border-yellow-200">
  <b>💡 Estrategia de Degradación:</b><br>
  "Devuelve siempre valor: datos esenciales + estado de componentes opcionales"
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🏆 ¿Qué hacen las empresas líderes?

## Observa los patrones comunes...

<div class="text-3xl mt-12">
¿Cómo manejan empresas como Amazon, Google y Stripe<br>
la exposición de inteligencia a clientes externos?
</div>

<div class="mt-10 text-2xl text-center">
<b>Analiza estos casos:</b>
<br>
• ¿Cómo exponen capacidades complejas manteniendo seguridad?<br>
• ¿Cómo evolucionan su lógica sin romper integraciones?<br>
• ¿Dónde trazan la línea entre interfaz y ejecución?
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🏆 Lecciones de las Grandes Plataformas

<div class="grid grid-cols-3 gap-6 mt-8">
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200 text-center">
    <div class="text-6xl mb-4">📦</div>
    <div class="text-2xl font-bold mb-2">Amazon Bedrock</div>
    <div class="text-lg">
      <b>Patrón:</b> API estandarizada<br>
      <b>Inteligencia:</b> Modelos ocultos<br>
      <b>Lección:</b> Contrato estable, implementación variable
    </div>
  </div>
  <div class="bg-purple-50 p-6 rounded-lg border border-purple-200 text-center">
    <div class="text-6xl mb-4">🛍️</div>
    <div class="text-2xl font-bold mb-2">Google Retail API</div>
    <div class="text-lg">
      <b>Patrón:</b> Capa de abstracción<br>
      <b>Inteligencia:</b> Recomendaciones internas<br>
      <b>Lección:</b> El cliente no ve cómo funciona
    </div>
  </div>
  <div class="bg-green-50 p-6 rounded-lg border border-green-200 text-center">
    <div class="text-6xl mb-4">💳</div>
    <div class="text-2xl font-bold mb-2">Stripe</div>
    <div class="text-lg">
      <b>Patrón:</b> Versionado inteligente<br>
      <b>Inteligencia:</b> Reglas de fraude ocultas<br>
      <b>Lección:</b> Evolución interna sin romper clientes
    </div>
  </div>
</div>

<div class="mt-10 text-3xl text-center bg-yellow-50 p-6 rounded-lg border border-yellow-200">
  <b>💡 Patrón Universal:</b><br>
  "Las interfaces estables exponen inteligencia oculta"
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🌟 ¿Qué otros dominios podríamos transformar?

## Piensa en tu área de trabajo...

<div class="text-3xl mt-12">
¿Qué otro dominio (logística, devoluciones,<br>
membresías) debería exponerse vía MCP<br>
con inteligencia interna?
</div>

<div class="mt-10 text-2xl text-center">
<b>Considera estos ejemplos:</b>
<br>
• Tiempo de entrega (logística externa + reglas internas)<br>
• Devoluciones (política pública + historial de cliente)<br>
• Ofertas personalizadas (datos externos + modelo interno)
</div>

---
theme: geist
colorSchema: light
layout: default
---

# ✅ Tesis Confirmada

<div class="text-3xl mt-8 text-center">
<b>El MCP Server es un puerto de I/O:</b><br>
expone, no ejecuta.
</div>

<div class="text-3xl mt-8 text-center">
<b>La Function Calling es ejecución local:</b><br>
piensa, decide, actúa.
</div>

<div class="text-3xl mt-8 text-center">
<b>Ambos son necesarios, distintos y complementarios.</b>
</div>

<div class="mt-16 grid grid-cols-3 gap-6">
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-blue-700">
      📐 Estándar MCP
    </div>
    <div class="text-xl">Definir contrato común para todos los servicios</div>
  </div>
  <div class="bg-purple-50 p-6 rounded-lg border border-purple-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-purple-700">
      🔁 Librería de Funciones
    </div>
    <div class="text-xl">Crear componentes inteligentes reutilizables</div>
  </div>
  <div class="bg-green-50 p-6 rounded-lg border border-green-200">
    <div class="text-2xl font-bold mb-4 flex items-center text-green-700">
      🚀 POC Inmediato
    </div>
    <div class="text-xl">Implementar con el caso del Shampoo Elvive</div>
  </div>
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🏆 Resumen Ejecutivo: El Patrón Ganador

<div class="text-3xl mt-8">
<b>El modelo perfecto para exponer inteligencia:</b>
</div>

<div class="grid grid-cols-2 gap-8 mt-8">
  <div class="bg-blue-50 p-8 rounded-lg border border-blue-200 text-center">
    <div class="text-6xl mb-4">🔌</div>
    <div class="text-2xl font-bold mb-4">MCP Server</div>
    <div class="text-xl">
      <b>ROL:</b> Adaptador universal<br>
      <b>FUNCION:</b> Contrato estable<br>
      <b>LÍMITE:</b> Sin lógica de negocio<br>
      <b>ANALOGÍA:</b> Puerto USB
    </div>
  </div>
  <div class="bg-purple-50 p-8 rounded-lg border border-purple-200 text-center">
    <div class="text-6xl mb-4">🧠</div>
    <div class="text-2xl font-bold mb-4">Function Calling</div>
    <div class="text-xl">
      <b>ROL:</b> Ejecutor inteligente<br>
      <b>FUNCION:</b> Lógica especializada<br>
      <b>LÍMITE:</b> Tiempos de respuesta<br>
      <b>ANALOGÍA:</b> Cerebro especializado
    </div>
  </div>
</div>

<div class="mt-12 text-4xl text-center bg-yellow-50 p-6 rounded-lg border border-yellow-200">
  <b>🚀 Fórmula de Éxito:</b><br>
  "Capa de exposición estandarizada + Inteligencia interna evolutiva"
</div>

---
theme: geist
colorSchema: light
layout: default
---

# 🙏 ¡Gracias por tu atención!

## Preguntas frecuentes

<div class="grid grid-cols-3 gap-6 mt-8">
  <div class="bg-blue-50 p-6 rounded-lg border border-blue-200">
    <div class="text-2xl font-bold mb-2">❓ ¿Puedo tener múltiples functions?</div>
    <div class="text-xl">Sí, el MCP puede orquestar múltiples funciones especializadas</div>
  </div>
  <div class="bg-purple-50 p-6 rounded-lg border border-purple-200">
    <div class="text-2xl font-bold mb-2">❓ ¿Cómo versiono el MCP?</div>
    <div class="text-xl">Con rutas /v1/ o headers, manteniendo compatibilidad hacia atrás</div>
  </div>
  <div class="bg-green-50 p-6 rounded-lg border border-green-200">
    <div class="text-2xl font-bold mb-2">❓ ¿Qué pasa con la latencia?</div>
    <div class="text-xl">Optimiza con timeouts, cache y modelos ligeros para cumplir SLAs</div>
  </div>
</div>

<div class="mt-12 text-3xl text-center">
<b>Próximos pasos:</b><br>
1. Definir estándar MCP para toda la organización<br>
2. Crear librería de funciones inteligentes<br>
3. Implementar POC con Shampoo Elvive
</div>

