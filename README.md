<p align="center">
  <img src="regiones/ATD_Loreto/logos/logo_gfp.png" alt="GFP Subnacional" height="88" />
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="regiones/ATD_Loreto/logos/logo_SECO.jpg" alt="Cooperación Suiza — SECO" height="72" />
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="regiones/ATD_Loreto/logos/logo_basel.png" alt="Basel Institute on Governance" height="72" />
</p>

<h1 align="center">ATD Toolbox ACR — Loreto, San Martín y Cusco</h1>

<p align="center">
  <strong>Caja de herramientas de Alertas Tempranas de Deforestación para Áreas de Conservación Regional</strong><br/>
  <em>GFP Subnacional · Suiza apoyando al Perú</em>
</p>

<p align="center">
  <a href="docs/GUIA_VISUAL.html"><strong>Guía de uso (HTML)</strong></a> ·
  <a href="INDICE.html">Índice por región</a>
</p>

<p align="center">
  <a href="#para-quién-es">Para quién es</a> ·
  <a href="#cómo-trabajar-en-3-pasos">Cómo trabajar</a> ·
  <a href="#así-se-ven-las-herramientas-por-dentro">Vista del toolbox</a> ·
  <a href="#demo-5-minutos">Demo 5 minutos</a> ·
  <a href="#las-tres-regiones">Las 3 regiones</a> ·
  <a href="#inicio-rápido">Inicio rápido</a>
</p>

---

## Para quién es

Para el **personal de las ACR** y equipos de monitoreo de Loreto, San Martín y Cusco.  
No necesita ser programador: solo **ArcGIS Pro 3.x** y seguir la guía HTML de **su** región.

---

## Cómo trabajar en 3 pasos

1. **Descargar alertas** desde Geobosques (H1)  
2. **Fotointerpretar** en el visor satelital y actualizar hectáreas (H2)  
3. Generar el **informe PDF oficial** (H3) **en su máquina** → carpeta `pdfs/`

| Paso | Herramienta | Qué hace |
|:----:|-------------|----------|
| **1** | **H1 — Descarga Geobosques** | Inserta alertas en la geodatabase de su región |
| **2** | **H2 — Visor + Actualizar Superficie** | Antes/después, recorte del polígono y hectáreas |
| **3** | **H3 — Reporte PDF** | Informe técnico con mapa, imágenes y logos institucionales |

<p align="center">
  <strong>Geobosques → H1 → H2 → H3 → PDF en <code>pdfs/</code> (local)</strong>
</p>

### Así se ven las herramientas (por dentro)

<p align="center">
  <img src="docs/guia/guia_h1_descarga_geobosques.png" alt="H1 — parámetros en ArcGIS Pro" width="520" />
</p>
<p align="center"><em>H1 — Descarga Geobosques (panel de geoprocesamiento)</em></p>

<p align="center">
  <img src="docs/guia/guia_h2_visor_antes_despues.png" alt="H2 — visor satelital antes/después" width="720" />
</p>
<p align="center"><em>H2 — Visor satelital (ANTES / DESPUÉS)</em></p>

<p align="center">
  <img src="docs/guia/guia_h2_visor_detalle.png" alt="H2 — detalle zoom sincronizado" width="720" />
</p>
<p align="center"><em>H2 — Zoom sincronizado para fotointerpretar</em></p>

> Los **PDF del reporte** los genera usted con H3 en su PC (`pdfs/`). No vienen listos en el repo.

---

## Demo 5 minutos

Prueba rápida **sin Geobosques** — el flujo es **igual** en las tres regiones; solo cambia la carpeta.

| Paso | Acción | Qué deberías ver |
|:----:|--------|------------------|
| 1 | Abrir **solo** `regiones/ATD_<Region>/` en ArcGIS Pro | Carpeta regional intacta |
| 2 | **Catalog → Add Toolbox** → H1, H2 y H3 en `toolbox/` | Las 3 herramientas |
| 3 | Agregar al mapa `GDB/…` → `MonitoreoDeforestacion` | Alertas en el mapa |
| 4 | **H2** → 1 polígono → escenas ANTES / DESPUÉS | Visor satelital GFP |
| 5 | **H3** → Diagnóstico Pre-Vuelo → Generar Reporte ATD | PDF nuevo en `pdfs/` |

```mermaid
flowchart LR
  A[H1 Geobosques] --> B[(MonitoreoDeforestacion)]
  B --> C[H2 Visor satelital]
  C --> D[imagenes_sentinel/ local]
  D --> E[H3 Reporte PDF]
  E --> F[pdfs/ local]
```

### Así sale el reporte (H3)

<p align="center">
  <img src="docs/guia/guia_h3_reporte_pdf.png" alt="Ejemplo reporte ATD — ANPCH Alto Nanay" width="820" />
</p>
<p align="center"><em>H3 — Reporte técnico ATD (ejemplo ANPCH · ACR Alto Nanay Pintuyacu Chambira)</em></p>

> Puede saltar **H1** si la GDB ya tiene alertas. En el repo solo hay esta **captura**; el PDF lo genera usted en `pdfs/` con H3.

---

## Las tres regiones

| Región | ACR | Carpeta | Guía HTML |
|--------|-----|---------|-----------|
| **Loreto** | CTT, Ampiyacu, Alto Nanay, Maijuna, MPA, ACM | [`regiones/ATD_Loreto/`](regiones/ATD_Loreto/) | [Guía](regiones/ATD_Loreto/guia/GUIA_ATD_LORETO.html) |
| **San Martín** | Cordillera Escalera (CE), BOSHUMI | [`regiones/ATD_San_Martin/`](regiones/ATD_San_Martin/) | [Guía](regiones/ATD_San_Martin/guia/GUIA_ATD_SAN_MARTIN.html) |
| **Cusco** | Choquequirao, Chuyapi Urusayhua, Q'eros Kosñipata | [`regiones/ATD_Cuzco/`](regiones/ATD_Cuzco/) | [Guía](regiones/ATD_Cuzco/guia/GUIA_ATD_CUZCO.html) |

Cada región trae: **toolbox H1–H2–H3**, **GDB**, **logos** (para el PDF) y **guía HTML**.  
**No mezclar** GDB ni logos entre GORE.

---

## Inicio rápido

1. Entrar a [`INDICE.html`](INDICE.html) y elegir **su región**.
2. **Descargar bien las GDB** (importante — ver abajo).
3. Abrir **solo** `regiones/ATD_<Region>/` en ArcGIS Pro.
4. **Catalog → Add Toolbox** → H1, H2 y H3 en `toolbox/`.
5. Ejecutar `DIAGNOSTICO_ENTORNO.bat` la primera vez.
6. Seguir la guía HTML de su región.

### ⚠️ Cómo descargar (si no, la GDB no abre)

Las geodatabases están en **Git LFS**. El botón **Code → Download ZIP** de GitHub **no trae los datos reales** (solo archivos de texto de ~130 bytes) y ArcGIS Pro muestra *File read/write error*.

**Forma correcta:**

```bat
git clone https://github.com/GFP-Subnacional-Peru/ATD-Toolbox-ACR.git
cd ATD-Toolbox-ACR
git lfs install
git lfs pull
```

O copiar la carpeta `regiones/ATD_<Region>/` desde un USB/paquete ya con LFS bajado.

**Comprobar:** en `GDB\…\*.gdbtable` el tamaño debe ser de **KB/MB**, no ~130 bytes. Si al abrir el archivo con Bloc de notas sale `version https://git-lfs.github.com/...`, la GDB está rota.

**Qué pesa:** geodatabases (datos) + logos + capturas del README.  
Para taller: puede copiar solo la carpeta de una región por USB.

---

## Créditos

**GFP Subnacional** · Cooperación Suiza (SECO) · Basel Institute on Governance  
GORE Loreto · GORE San Martín · GORE Cusco

<sub>Versión 2026 · Uso institucional ATD ACR · Sin reportes pregenerados</sub>
