# 💧 FuenteGo (Proyecto en Producción)

🌐 **Sitio web en vivo:** [fuentego.com](https://fuentego.com)

> 🔒 **Nota de Seguridad:** El código fuente de este proyecto es privado ya que actualmente es un producto en producción desplegado mediante Cloudflare. Este repositorio sirve como un escaparate técnico (Showcase) de la arquitectura y las tecnologías utilizadas.

## 🚀 Sobre el Proyecto
**FuenteGo** es una suite de herramientas web diseñada para gamers y usuarios de redes sociales que buscan destacar su identidad digital. Resuelve el problema de los nombres de usuario ocupados o monótonos ofreciendo generadores avanzados de nicks, fuentes Unicode y catálogos de símbolos *aesthetic* listos para copiar y pegar en múltiples idiomas.

## 🛠️ Arquitectura y Tech Stack
* **Frontend:** [Astro](https://astro.build/) (SSG), TypeScript, HTML/CSS nativo y Vanilla JS.
* **Internacionalización (i18n):** Sistema de enrutamiento SEO-friendly en 4 idiomas (ES, EN, PT, FR).
* **SEO y Marcado:** Inyección dinámica de metadatos y schemas JSON-LD (FAQPage, WebApplication, ItemList).
* **Despliegue y CI/CD:** Cloudflare Pages impulsado por GitHub Actions para integración y despliegue continuo.

## 💡 Retos Técnicos Superados
* **SEO a Gran Escala e Internacionalización:** Implementación de generación de rutas estáticas (`getStaticPaths` en Astro) acoplada a un sistema robusto de diccionarios en TypeScript. Se integraron *Rich Snippets* dinámicos (FAQ Schemas) para acaparar mayor espacio visual en las SERPs móviles de Google y aumentar drásticamente el CTR en distintos países.
* **Rendimiento y Core Web Vitals:** Las herramientas de transformación de texto (fuentes raras, algoritmos de generación aleatoria y detectores de "shake" en móviles) se construyeron utilizando Vanilla JS sin frameworks pesados. Esto asegura un "Zero-JS payload" inicial, logrando puntuaciones perfectas en Lighthouse y tiempos de carga instantáneos apoyados por la CDN global de Cloudflare.
* **Arquitectura Escalable de Datos:** Separación estricta entre la lógica de interfaz de usuario y los conjuntos de datos (listas de sufijos, clanes, arrays de símbolos y traducciones) usando interfaces de TypeScript, permitiendo escalar a nuevos juegos o idiomas sin refactorizar los componentes visuales.

## 📸 Capturas de Pantalla
<img width="1313" height="965" alt="image" src="https://github.com/user-attachments/assets/9bf78a8b-2b3a-4946-ad83-40568a915152" />
<img width="1501" height="906" alt="image" src="https://github.com/user-attachments/assets/9d8d33c8-efbc-4fa1-93f3-bd18b30eb0f8" />
<img width="1257" height="957" alt="image" src="https://github.com/user-attachments/assets/b72be532-f5e3-44d1-82b4-34ed744af27a" />
