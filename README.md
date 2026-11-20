# Ju-bits

**Tu compañero de estudio con IA** · Instituto Juventud del Estado de México

Ju-bits es una versión en miniatura de un tutor con inteligencia artificial para estudiantes de preparatoria. Cada estudiante le da vida con **su propia clave gratuita, de Groq o de Gemini** (él elige el motor), y escoge con quién estudiar entre cuatro compañeros, cada uno con su bolita:

| Compañero | Personalidad | Color |
|---|---|---|
| **Pete** | Fuerte y confiable | Verde |
| **Mary** | Empática y erudita | Azul |
| **Joss** | Creativo e innovador | Violeta |
| **Vily** | Sabio y meditativo | Amarillo |
| **Adv** | Paz y tradición decembrina | Rojo navideño |

Adv es el compañero especial de diciembre: experto en las festividades y tradiciones católicas de ese mes, con la descripción «Disponible hasta el 7 de enero»; pasado ese día, su tarjeta deja de mostrarse.

Los cuatro comparten la misma misión: ayudar a **estudiar y entender** — explicar paso a paso, guiar con preguntas y resolver *con* el estudiante, no *por* él — con la identidad y el trato del Instituto Juventud del Estado de México.

## Cómo se usa

1. Abre la página de Ju-bits.
2. Elige tu motor: **Groq** o **Gemini**, y pega tu clave. ¿No tienes? Es gratis en ambos casos:
   - Groq: [console.groq.com/keys](https://console.groq.com/keys) — crea tu cuenta, pulsa **Create API Key** y cópiala (empieza con `gsk_`).
   - Gemini: [aistudio.google.com/apikey](https://aistudio.google.com/apikey) — entra con tu cuenta de Google, pulsa **Create API key** y cópiala (empieza con `AIza`).
3. Elige a tu compañero: Pete, Mary, Joss o Vily (y en diciembre, también Adv).
4. Escribe tu duda o el tema que quieres estudiar.

## Privacidad

- La clave (de Groq o de Gemini) se guarda **únicamente en el navegador del estudiante** (`localStorage`). Nunca se envía a ningún servidor distinto del de Groq, y este proyecto no tiene servidor propio.
- Las conversaciones tampoco se guardan: al cerrar la pestaña, se van.

## Tecnología

- Una sola página (`index.html`), sin dependencias: HTML, CSS y JavaScript.
- Llama directamente a la API que el estudiante elija: Groq (compatible con OpenAI, modelo `llama-3.1-8b-instant`) o Gemini (modelo `gemini-2.5-flash`). Los modelos se cambian en las funciones `askGroq` y `askGemini` de `index.html`.
- Los cuatro compañeros son imágenes (`pedro.jpg`, `mary.jpg`, `joss.jpg`, `iram.jpg`): muñecos de tela con ojos de botón, uno de cada color, con las letras JB en el pecho.
- Pensado para publicarse con GitHub Pages.

## Créditos

Proyecto educativo del **Instituto Juventud del Estado de México**.

*Construirse es construir el mundo.*
