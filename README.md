<p align="center">
  <img src="regiones/ATD_Loreto/logos/logo_gfp.png" alt="GFP Subnacional" height="80" />
</p>

<h1 align="center">ATD Toolbox ACR — Loreto, San Martín y Cusco</h1>

<p align="center">
  <strong>Caja de herramientas de Alertas Tempranas de Deforestación para Áreas de Conservación Regional</strong><br/>
  <em>GFP Subnacional · Suiza apoyando al Perú</em>
</p>

<p align="center">
  <a href="#regiones">Regiones</a> ·
  <a href="#inicio-rápido">Inicio rápido</a> ·
  <a href="INDICE.html">Índice HTML</a>
</p>

---

## ¿Qué es este repositorio?

Paquete **institucional** del flujo ATD (Alertas Tempranas de Deforestación) en **Áreas de Conservación Regional** de tres regiones del Perú. Cada región es un paquete autocontenido para ArcGIS Pro 3.x con geodatabases, toolbox H1–H3, logos y guías.

| Región | Carpeta | ACR |
|--------|---------|-----|
| **Loreto** | [`regiones/ATD_Loreto/`](regiones/ATD_Loreto/) | ACR04 CTT · ACR09 Ampiyacu · ACR10 Alto Nanay · ACR17 Maijuna · ACR34 MPA · ACR37 ACM |
| **San Martín** | [`regiones/ATD_San_Martin/`](regiones/ATD_San_Martin/) | ACR01 Cordillera Escalera · ACR21 BOSHUMI |
| **Cusco** | [`regiones/ATD_Cuzco/`](regiones/ATD_Cuzco/) | ACR07 Choquequirao · ACR26 Chuyapi Urusayhua · ACR30 Q'eros Kosñipata |

### Herramientas (por región — mismos arreglos 2026)

| | Herramienta | Función |
|---|-------------|---------|
| **H1** | Descarga Geobosques | Inserta alertas en la GDB |
| **H2** | Visor satelital + Actualizar Superficie (ha) | Fotointerpretación antes/después; hectáreas tras recorte |
| **H3** | Reporte PDF | Diagnóstico + informe (Causa→Actividad; efecto = pérdida de hábitat; md_sup 2 decimales) |

**Flujo:** Geobosques → H1 → H2 (visor → recorte → Actualizar Superficie) → H3 PDF.

No mezclar GDB ni logos entre regiones.

---

## Inicio rápido

1. Elija su región en [`INDICE.html`](INDICE.html) o entre a `regiones/ATD_<Region>/`.
2. Abra **solo esa carpeta** en ArcGIS Pro (no mueva el toolbox fuera).
3. **Catalog → Add Toolbox** → los tres `.pyt` en `toolbox/`.
4. Lea `guia/GUIA_ATD_<REGION>.html` de la región elegida.
5. Ejecute `DIAGNOSTICO_ENTORNO.bat` antes del primer uso.

---

## Paquetes relacionados

| Recurso | Uso |
|---------|-----|
| Este repo (`ATD-Toolbox-ACR`) | Las 3 regiones juntas |
| [ATD-Loreto-GFP](https://github.com/Favio138-hub/ATD-Loreto-GFP) | Solo Loreto |

---

## Créditos

**GFP Subnacional** · GORE Loreto, San Martín y Cusco · SECO / Basel Institute

<sub>Versión 2026 · Uso institucional ATD ACR</sub>
