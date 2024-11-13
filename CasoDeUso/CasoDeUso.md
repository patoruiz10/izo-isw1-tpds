**Caso de Uso: Cámara Vial**

**Primario: Cámara**

**Pre-Condiciones:** Tiene que transitar un vehículo por delante de la cámara

**Camino básico**:

1\. La cámara envía los datos al sistema

2\. El sistema recibe los datos del vehículo.

**Camino alternativo:**

2a. El sistema no recibe ningún dato del vehículo

2b. Si la velocidad es mayor a los 70km/h, el sistema envía los datos a una API, que se encarga de guardar los datos en una base de datos. Además envía un correo con los datos que envió la cámara a una cuenta “aviso@ciudad”

2c. Si la velocidad es mayor a los 100km/h, el sistema envía los datos a una API, que se encarga de guardar los datos en una base de datos. Además envía un correo con los datos que envió la cámara a una cuenta “aviso@ciudad”. El sistema envía 3 veces los datos recibidos por la cámara a un impresora para que sean impresos

**Escenario de éxito:**

\- El sistema recibe los datos de la cámara y los almacena

**Escenario de fracaso:**

\- No recibe datos del vehículo

