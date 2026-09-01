## 3.2 Historias de usuario

En esta sección se definen las Historias de Usuario (User Stories) estructuradas en función de los dos segmentos objetivo de Veygo: **Clientes (Arrendatarios)** y **Propietarios (Arrendadores)**. Cada historia sigue el formato estándar (*Como [Rol] Quiero [Acción] Para [Beneficio]*) e incluye sus respectivos criterios de aceptación bajo la estructura BDD (*Dado que / Cuando / Entonces*).

---

### 3.2.1. Tabla de Épicos del Proyecto Veygo

| ID de Épico | Título | Descripción |
| :--- | :--- | :--- |
| *EP-01* | Landing Page y Captura de Interés | Página pública de inicio para presentar los beneficios de Veygo, testimonios, formulario de contacto y llamados a la acción para registrarse como cliente o propietario. |
| *EP-02* | Registro, Autenticación y Verificación de Identidad | Creación de cuenta, inicio de sesión seguro y verificación documental de identidad (DNI/Brevete) para garantizar transacciones confiables entre usuarios. |
| *EP-03* | Búsqueda Geolocalizada y Mapa de Cercanía | Implementación del mapa interactivo en tiempo real para visualizar vehículos (autos y motos) disponibles cercanos a la ubicación de entrega del cliente. |
| *EP-04* | Filtros Avanzados de Vehículos | Sistema de filtrado por tipo de vehículo (auto/moto), transmisión (manual/automática), motorización (eléctrica/combustible) y rango de precio. |
| *EP-05* | Gestión de Publicaciones de Vehículos | Flujo para que los propietarios puedan registrar, editar y gestionar sus vehículos, subiendo características, tarifas e imágenes. |
| *EP-06* | Calendario Dinámico y Gestión de Disponibilidad | Control de fechas en tiempo real para evitar solapamientos de reservas y permitir al propietario gestionar la disponibilidad de su flota. |
| *EP-07* | Proceso de Reserva y Gestión de Solicitudes | Flujo completo para que el cliente solicite un vehículo, confirme fechas de alquiler y reciba la validación del propietario sin canales informales. |
| *EP-08* | Panel Administrativo y Métricas para Propietarios | Dashboard privado para propietarios con visión general de vehículos activos, total de transacciones completadas e ingresos generados. |
| *EP-09* | Sistema de Calificaciones, Reseñas y Reputación | Evaluaciones bidireccionales post-alquiler para construir confianza dentro del ecosistema de Veygo. |
### 3.2.2. Detalle de Historias de Usuario

#### EP-02: Registro, Autenticación y Verificación de Identidad

| ID | Historia de Usuario | Criterios de Aceptación (BDD) |
| :--- | :--- | :--- |
| **US-01** | **Como:** Cliente o propietario registrado[cite: 2].<br>**Quiero:** Subir mi documento oficial de identidad (DNI) y Licencia de Conducir a la plataforma[cite: 2].<br>**Para:** Validar mi identidad antes de realizar transacciones de alquiler y generar confianza en la comunidad[cite: 2]. | **Dado que** el usuario registrado ingresa a su perfil y no cuenta con verificación de identidad[cite: 2],<br>**Cuando** cargue las fotos legibles del anverso y reverso de su DNI y Brevete vigente,<br>**Entonces** el sistema cambiará el estado de la cuenta a "En Verificación" y emitirá una notificación de confirmación al completar la validación. |
| **US-02** | **Como:** Usuario registrado (Cliente o Propietario)[cite: 2].<br>**Quiero:** Iniciar sesión con mi correo electrónico y contraseña o autenticación rápida.<br>**Para:** Acceder de forma segura a mi perfil, publicaciones y reservas activas[cite: 2]. | **Dado que** el usuario ingresa a la pantalla de inicio de sesión[cite: 2],<br>**Cuando** ingrese credenciales válidas,<br>**Entonces** el sistema le otorgará acceso y lo redirigirá a su tablero principal según su rol. |

---