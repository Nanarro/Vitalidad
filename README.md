# 🎹 Vitalidad

**Vital en tu iPad, sin Mac y sin gastar de más.**

Este repositorio compila [Vital](https://github.com/mtytel/vital) (el sintetizador de wavetables de Matt Tytel) para iPad como app y plugin **AUv3**, usando un Mac virtual gratuito de GitHub Actions. Así puedes cargarlo dentro de GarageBand u otros hosts compatibles con AUv3.

> ⚠️ **Estado: experimental.** El flujo de compilación todavía no está probado de punta a punta. Si algo falla, el log te dice dónde.

---

## ✨ ¿Qué hace?

1. Descarga el código oficial de Vital.
2. Ajusta el proyecto de Xcode para que compile con herramientas modernas.
3. Compila para iPad (arm64) **sin firmar**.
4. Te entrega un archivo `Vital-unsigned.ipa`.

---

## 🚀 Cómo usarlo (desde el navegador del celular)

1. Abre la pestaña **Actions** de este repositorio.
2. Elige **Build Vital iOS (AUv3)**.
3. Pulsa **Run workflow** y espera (puede tardar bastante).
4. Al terminar, baja los **artifacts**:
   - `Vital-unsigned-ipa` → el instalador.
   - `build-log` → el registro, útil si algo falló.

> Si falla, comparte el `build-log` con quien te ayuda (o con Claude) y se corrige el workflow.

---

## 📲 Instalarlo en el iPad

El `.ipa` sale **sin firmar**, así que hay que firmarlo e instalarlo con una herramienta de *sideloading*:

| Opción | Costo | Notas |
|---|---|---|
| **Sideloadly** / **AltStore** con Apple ID gratis | Gratis | Necesita una PC o Mac al menos la primera vez. La app caduca cada **7 días** y hay que reinstalarla. |
| **Apple Developer Program** | ~99 USD/año | La firma dura un año y permite TestFlight. |

Después de instalar, abre GarageBand (o tu host AUv3) y busca **Vital** entre los instrumentos de Audio Unit.

---

## 🎛️ Presets y wavetables

El código de Vital en GitHub **no incluye presets ni wavetables**. Descarga presets gratuitos de la comunidad y respeta la licencia de cada pack.

---

## 🧩 Alternativas si esto no te funciona

- Usar Vital en una PC o Mac prestada, exportar audio y cargarlo en **Koala Sampler** o **FL Studio Mobile**.
- Sintetizadores AUv3 baratos para iPad, usados dentro de **GarageBand** (gratis).

---

## ⚖️ Licencia y créditos

- **Vital** es de Matt Tytel y se distribuye bajo **GPLv3**.
- Por esa licencia, **no se puede publicar en la App Store**. Este proyecto es para uso personal.
- No subas ni compartas builds que incluyan presets o wavetables de terceros con licencia restringida.
- Este repositorio no está afiliado a Vital Audio ni a Anthropic.

Hecho con paciencia, café y ganas de hacer música. 🎶
