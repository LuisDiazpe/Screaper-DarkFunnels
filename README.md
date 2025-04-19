# Screaper-DarkFunnels

## 🧠 ¿Qué es esto?

Este proyecto es un **robot inteligente** que busca negocios en Google Maps, extrae datos importantes (como teléfonos, sitios web y redes sociales), y los guarda de forma ordenada en una base de datos.

Funciona con solo darle una frase como:

> “Busca dentistas en San Isidro”

---

## 🧩 ¿Cómo funciona? (Explicado simple pero profesional)

### 1. 🗨️ Recibe tu mensaje

Le das una frase como si hablaras con un asistente virtual.  
El robot analiza tu mensaje y detecta:

- 🏙️ El **distrito** (ej. San Isidro)
- 🏪 El **rubro** (ej. dentistas)

---

### 2. 🌍 Busca en Google Maps

Usa Google Maps para encontrar negocios que coincidan con el distrito y rubro que solicitaste.

---

### 3. 🎯 Filtra y valida

- Verifica que el distrito y rubro existan.
- Si hay errores, responde con un **mensaje claro**.
- Calcula la **cantidad de páginas** que debe revisar según el tamaño del distrito.

---

### 4. 🔌 Llama a la API

Usa una API para extraer todos los negocios relacionados con tu búsqueda.

---

### 5. 📥 Guarda la información

Guarda los datos extraídos (nombre, dirección, teléfono, etc.) en una **base de datos**.

---

## 🕸️ Procesamiento de enlaces

- Intenta conseguir la **página web** de cada negocio.
- Revisa si la página **funciona** o está caída.
- Filtra links inválidos, como:
  - Páginas de Facebook
  - Enlaces generados incorrectamente
  - Enlaces rotos o vacíos
- Intenta **completar o corregir** enlaces incompletos.

---

## 🕵️‍♂️ Scraping de páginas web

- Abre cada página web y revisa su **código fuente**.
- Espera **10 segundos** entre cada página para evitar sobrecargas.
- Busca **números telefónicos, correos y redes sociales**.
- Si encuentra múltiples teléfonos, los combina ordenadamente.

---

## 🗂️ Organización final

- Toda la información se presenta **ordenada y clara** para el usuario final.
- Se capturan y reportan **errores o datos faltantes**.

---

---

## 💬 Ejemplo de uso al devolver la información al usuario
{ "texto": "🔹 Negocio 1:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51994182204\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/odontologistsperu\n• Instagram: https://www.instagram.com/clinica_dental_odontologists/\n\n---\n\n🔹 Negocio 2:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• WhatsApp: +5151943512277\n• Móvil: +51943512277\n• Móvil: +51980285355\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/sharer/sharer.php\n• Twitter: https://twitter.com/intent/tweet\n\n---\n\n🔹 Negocio 3:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• WhatsApp: +5151947991170\n• Móvil: +51947991170\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/Mundoral\n• Instagram: https://www.instagram.com/mundoralodontologos/\n• TikTok: https://www.tiktok.com/@mundoral_odontologos\n\n---\n\n🔹 Negocio 4:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51939365038\n• Móvil: +51951389541\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/tr\n• Instagram: https://www.instagram.com/clinicaodontologicalservices/\n• TikTok: https://www.tiktok.com/@odontologicalservices\n\n---\n\n🔹 Negocio 5:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51997731085\n\n📲 Redes Sociales:\n• Facebook: https://facebook.com/Vanedent\n• Instagram: https://instagram.com/Vanedent\n• TikTok: https://tiktok.com/@vanedent.peru\n\n---\n\n🔹 Negocio 6:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51991216060\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/dentistaenmirafloreslim\n• Instagram: https://www.instagram.com/odontodigital3/\n\n---\n\n🔹 Negocio 7:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51941310513\n\n📲 Redes Sociales:\nNo disponible\n\n---\n\n🔹 Negocio 8:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51969274133\n• Teléfono Fijo: +5117482911\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/laserdentkidsperu/\n• Instagram: https://www.instagram.com/laserdentkidsoficial\n• TikTok: https://www.tiktok.com/@laserdentkids\n\n---\n\n🔹 Negocio 9:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• WhatsApp: +51970578659\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/clinicasonrisanas\n\n---\n\n🔹 Negocio 10:\n🌐 Website: No disponible\n\n📞 Teléfonos:\nNo disponible\n\n📲 Redes Sociales:\nNo disponible\n\n---\n\n🔹 Negocio 11:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51969274133\n• Teléfono Fijo: +5117482911\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/laserdentkidsperu/\n• Instagram: https://www.instagram.com/laserdentkidsoficial\n• TikTok: https://www.tiktok.com/@laserdentkids\n\n---\n\n🔹 Negocio 12:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• WhatsApp: +5151989507460\n• Móvil: +51989507460\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/NeodentisPeru\n\n---\n\n🔹 Negocio 13:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51920404656\n• Móvil: +51959044042\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/midentistaperu\n• Instagram: https://www.instagram.com/midentista.pe/\n• TikTok: https://www.tiktok.com/@midentistaperu\n\n---\n\n🔹 Negocio 14:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51950564003\n• Móvil: +51923768962\n• Móvil: +51942793449\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/dentalhousekidsodontopediatria\n• Instagram: https://instagram.com/dentalhousekidsperu\n• TikTok: https://www.tiktok.com/@dentalhousekids\n\n---\n\n🔹 Negocio 15:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• Móvil: +51993150065\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/DentistasEspecialistasEnBrackets\n• Instagram: https://www.instagram.com/atracciondental.pe/\n• TikTok: https://www.tiktok.com/@atracciondental.pe\n\n---\n\n🔹 Negocio 16:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• WhatsApp: +5151932823498\n• Móvil: +51932823498\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/bluesmiledent\n• Instagram: https://www.instagram.com/bluesmile.peru/\n• TikTok: https://www.tiktok.com/@bluesmile.pe\n\n---\n\n🔹 Negocio 17:\n🌐 Website: No disponible\n\n📞 Teléfonos:\n• WhatsApp: +5151923982806\n• Móvil: +51923982806\n\n📲 Redes Sociales:\n• Facebook: https://www.facebook.com/odontologiaesteticaperu\n• Instagram: https://www.instagram.com/odontologoandrea_peru\n• TikTok: https://www.tiktok.com/@odontologoandrea_peru\n\n---" }
