# 🎧 Wenavolá — Radio Online & Plataforma de Contenidos

Wenavolá es una radio online + plataforma editorial enfocada en música, cultura urbana y contenidos digitales.
Este repositorio contiene el frontend desarrollado en **Next.js**, consumiendo datos desde un CMS **WordPress Headless** vía **GraphQL**.

---

## 🚀 Stack Tecnológico

* **Frontend:** Next.js (React)
* **CMS:** WordPress (Headless)
* **API:** WPGraphQL
* **Deploy:** Vercel
* **Estilos:** (Tailwind CSS / CSS Modules — definir)
* **Lenguaje:** TypeScript (recomendado)

---

## 🌐 Arquitectura

Usuario → Frontend (Next.js en Vercel) → GraphQL → WordPress CMS

* El contenido (artistas, programas, podcasts, noticias) se gestiona en WordPress
* El frontend consume los datos vía endpoint GraphQL

---

## 📦 Instalación

Clona el repositorio:

```bash
git clone https://github.com/tu-usuario/wenavola-web.git
cd wenavola-web
```

Instala dependencias:

```bash
npm install
```

---

## ⚙️ Variables de entorno

Crea un archivo `.env.local` en la raíz:

```env
NEXT_PUBLIC_GRAPHQL_ENDPOINT=https://cms.wenavola.cl/graphql
```

---

## 🧪 Desarrollo

```bash
npm run dev
```

App disponible en:

```
http://localhost:3000
```

---

## 📡 Ejemplo de Query GraphQL

```graphql
query GetArtistas {
  artistas {
    nodes {
      nombreArtistico
      instagram
      biografia
    }
  }
}
```

---

## 🧩 Estructura del Proyecto

```
/src
  /components   → Componentes reutilizables
  /pages        → Rutas (Next.js)
  /lib          → Configuración API / GraphQL
  /styles       → Estilos globales
  /hooks        → Custom hooks
```

---

## 🎯 Roadmap

* [ ] Landing principal (Hero + Radio en vivo)
* [ ] Página de artistas
* [ ] Página de programas
* [ ] Podcasts
* [ ] Blog / noticias
* [ ] Player de radio persistente
* [ ] SEO + performance

---

## 📻 Features principales

* Streaming de radio en vivo
* Contenido editorial dinámico
* Integración con redes sociales
* Plataforma escalable

---

## 🤖 Uso con IA (Codex / ChatGPT)

Este proyecto está optimizado para trabajar con asistentes de código:

Ejemplos de prompts:

* "Crea componente de lista de artistas usando GraphQL"
* "Optimiza este fetch de datos en Next.js"
* "Agrega SSR para esta página"

---

## 🚀 Deploy

Deploy automático con Vercel:

1. Conectar repositorio
2. Configurar variables de entorno
3. Deploy

---

## ⚠️ Consideraciones

* No subir archivos `.env`
* Mantener endpoints seguros
* Validar datos desde CMS

---

## 🧑‍💻 Autor

Proyecto desarrollado por Wenavolá
Radio digital & plataforma cultural

---

## 📄 Licencia

MIT
