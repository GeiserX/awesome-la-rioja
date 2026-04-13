# AGENTS.md — awesome-la-rioja

## Propósito

Selección de software open source que da **soporte específico a La Rioja** — su gobierno autonómico, ayuntamientos, universidades, empresas, infraestructuras y patrimonio. Todo el contenido en español. El foco es La Rioja: el software debe dirigirse específicamente a esta comunidad autónoma o a sus municipios.

## Ámbito

- **La Rioja es una comunidad autónoma uniprovincial** con 174 municipios.
- Principales ciudades: Logroño (capital), Calahorra, Arnedo, Haro, Alfaro, Nájera, Santo Domingo de la Calzada, Lardero, Villamediana de Iregua, Autol, Pradejón, Rincón de Soto, Fuenmayor, Navarrete, Cenicero, San Asensio, Ezcaray.
- **Universidades**: UR (Universidad de La Rioja).
- **Instituciones**: Gobierno de La Rioja, IDERioja (Infraestructura de Datos Espaciales de La Rioja), ADER (Agencia de Desarrollo Económico de La Rioja), ODS La Rioja (Objetivos de Desarrollo Sostenible), SOS Rioja.

## Criterios de inclusión

### Incluir

- Software que interactúa con el **Gobierno de La Rioja** o sus organismos (Sede Electrónica, Portal de Transparencia, datos abiertos).
- Herramientas para **ayuntamientos** de La Rioja.
- Software de **universidades riojanas** (UR) cuando sea específico de la región o la universidad.
- Herramientas de **datos abiertos** de La Rioja (datos.larioja.org).
- Software relacionado con **IDERioja** (cartografía, SIG, geodatos, API de mapas).
- Herramientas de **meteorología** regional (estaciones del Gobierno de La Rioja, SOS Rioja).
- Software sobre la **DOCa Rioja** (denominación de origen, viticultura, enología).
- Herramientas de **cartografía y SIG** específicas de La Rioja (IDERioja, LiDAR, GeoJSON).
- Software de **transporte** riojano (autobuses interurbanos, movilidad).
- Herramientas de **turismo y patrimonio** de la región (Camino de Santiago, monasterios, dinosaurios).
- Software de **medio ambiente** regional (Ebro, espacios naturales, calidad del aire).
- Proyectos de **smart cities** para ciudades riojanas.
- Software sobre **deportes** riojanos.
- Proyectos del **sistema sanitario riojano** (SERIS).
- Software **educativo** específico de la región.
- Herramientas de **industria y empresa** riojana (ADER, calzado en Arnedo, conservas en Calahorra).
- Proyectos de **ODS** (Objetivos de Desarrollo Sostenible) de La Rioja.
- Herramientas de **IoT y LoRaWAN** específicas de La Rioja (TTN Logroño).

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de La Rioja — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por riojanos que **no tiene funcionalidad específica** de la región.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.

### Zona gris — usar criterio

- Proyectos de la Universidad de La Rioja que podrían ser genéricos — incluir si tienen datos o configuración específica de La Rioja.
- Software que cubre La Rioja junto con otras regiones — incluir si La Rioja es un foco principal.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución riojana** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `###`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-la-rioja» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades riojanas (Reddit, foros de la UR, grupos de desarrolladores riojanos) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- La Rioja es una comunidad autónoma uniprovincial y pequeña. El ecosistema de software open source es reducido comparado con comunidades más grandes.
- **IDERioja** (iderioja en GitHub) es la principal fuente de repos institucionales. Tiene 11 repositorios de cartografía, geodatos y documentación de APIs. Ninguno tiene licencia explícita en GitHub.
- **goiblas/open-data-la-rioja** es el repo con más estrellas (19) relacionado con La Rioja: visualización de datos abiertos del Gobierno de La Rioja.
- **ods-larioja** es una organización con repos de staging para los Objetivos de Desarrollo Sostenible de La Rioja.
- **GobiernoLaRioja** tiene organización en GitHub pero solo un repo (página web estática, sin actividad desde 2018).
- La Universidad de La Rioja (UR / UNIR) no tiene organización oficial en GitHub. Los repos encontrados son ejercicios de clase sin utilidad real.
- No confundir UNIR (Universidad Internacional de La Rioja, online, genérica) con UR (Universidad de La Rioja, presencial, local). Solo UR es relevante.
- **auva/riojac**: descarga de temperaturas de estaciones meteorológicas del Gobierno de La Rioja. GPL-3.0, Java, pero sin actividad desde 2015.
- **jecrespo/TTN-Logrono**: comunidad The Things Network de Logroño para IoT/LoRaWAN. GPL-3.0, C++.
- Las búsquedas de "Logroño" en GitHub devuelven muchos resultados irrelevantes (apellidos, ciudades de Latinoamérica con nombre similar).
- Las búsquedas de "rioja" devuelven mucho ruido (vino genérico, Argentina - La Rioja provincia).
- **Rate limits**: el API de búsqueda de GitHub (30 req/min) se agota rápido. Usar `gh api repos/...` (core API, 5000/h) para verificar repos concretos.

*Generated by [LynxPrompt](https://lynxprompt.com) CLI*
