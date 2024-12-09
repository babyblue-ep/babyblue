# Proyecto Baby Blue

**Baby Blue** es un dispositivo de medición de **EEG** de un solo canal, ultra low power y de código abierto.

---

## Características

- **Código abierto**: Todos los archivos están disponibles en nuestro [repositorio](https://github.com/babyblue/project).
- **Ultra low power**: Diseñado para maximizar la eficiencia energética.
- **Bajo costo**: Accesible para investigadores y estudiantes.

---

## Evolución del Dispositivo

1. **Versión 1.0**:
   - Prototipo inicial.
   - Diseño funcional básico.

2. **Versión 2.0**:
   - Incorporación de componentes de bajo consumo.
   - Mejoras en la precisión del muestreo.

3. **Versión 3.0** (en desarrollo):
   - Reducción de tamaño.
   - Conexión inalámbrica mediante **Bluetooth**.

---

## Publicaciones

> Hemos publicado investigaciones en revistas especializadas sobre el uso de Baby Blue en mediciones de EEG.

| Año | Título de la Publicación                   | Revista/Conferencia       |
|-----|-------------------------------------------|---------------------------|
| 2023 | Baby Blue: A Low-Cost EEG Device          | Journal of NeuroTech      |
| 2024 | Ultra Low-Power EEG Systems for Research | International EEG Summit  |

---

## Diseño

![Esquema del Diseño](https://example.com/blueprint.jpg)

El diseño incluye:
- Un amplificador de señal de bajo ruido.
- Un procesador ultra low power.
- Batería de larga duración.

Puedes descargar los archivos de diseño [aquí](https://github.com/babyblue/design).

---

## Tienda

¡Adquiere tu dispositivo Baby Blue ahora!  
Visita nuestra tienda en [https://babyblue-store.com](https://babyblue-store.com).

---

## Código de Ejemplo

Aquí tienes un fragmento de código para configurar el dispositivo:

```cpp
#include <BabyBlue.h>

void setup() {
  BabyBlue.begin();
  BabyBlue.setSamplingRate(256);
}

void loop() {
  float eegData = BabyBlue.readEEG();
  Serial.println(eegData);
}
