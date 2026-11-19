# Dolores AR

App turística con realidad aumentada para visitar Dolores Hidalgo, construida con TDD (ROJO, VERDE, REFACTOR).


## 1. Distancia (Haversine)

### ROJO: la prueba falla porque `distanciaMetros` todavía no existe en `geo.dart`.

![Distancia rojo](assets/R1_ROJO_distancia.png)


## 2. Rumbo y ángulos

### ROJO: la prueba falla porque faltan `rumboGrados`, `normalizar360`, `diferenciaAngular` y `suavizarAngulo`.

![Rumbo y ángulos rojo](assets/R2_ROJO_rumbo-angulos.png)


## 3. Campo de visión

### ROJO: la prueba falla porque faltan `posicionHorizontal`, `formatearDistancia` y `nombreCardinal`.

![Campo de visión rojo](assets/R3_ROJO_campo-vision.png)


## 4. Motor de realidad aumentada

### ROJO: la prueba falla porque `motor_ar.dart` todavía no existe.

![Motor AR rojo](assets/R4_ROJO_motor-ar.png)

### VERDE: se implementa `calcularVisibles` y pasan las 9 pruebas del motor.

![Motor AR verde](assets/R4_VERDE_motor-ar.png)


## 5. Pasaporte turístico

### ROJO: la prueba falla porque la clase `Pasaporte` todavía no existe.

![Pasaporte rojo](assets/R5_ROJO_pasaporte.png)

### VERDE: se implementa `Pasaporte` (sello a menos de 40 m, una sola vez) y pasan las 5 pruebas.

![Pasaporte verde](assets/R5_VERDE_pasaporte.png)


## 6. Fuentes de datos y ViewModel

### ROJO: la prueba falla porque faltan los contratos, las excepciones y `ArViewModel`.

![ViewModel rojo](assets/R6_ROJO_viewmodel.png)

### VERDE: se implementa el ViewModel con fuentes falsas y pasan las 8 pruebas.

![ViewModel verde](assets/R6_VERDE_viewmodel.png)


## 7. Resultado final

### VERDE: las 43 pruebas del proyecto pasan juntas con `flutter test`.

![Todas las pruebas](assets/RF_VERDE_todas-las-pruebas.png)


## 8.Resultado de las pantallas
### Explorar con GPS real
<img src="assets/modo_demo.jpeg" alt="Explorar con gps real" width="250" />

### Modo demo
<img src="assets/GPS_real.jpeg" alt="Modo demo" width="250" />
