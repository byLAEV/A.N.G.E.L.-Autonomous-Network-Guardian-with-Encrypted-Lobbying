# A.N.G.E.L.-Autonomous-Network-Guardian-with-Encrypted-Lobbying
Sistema de seguridad de red innovador que utiliza inteligencia artificial para fragmentar la red en lobbys virtuales aislados. Acceso controlado mediante claves temporales cifradas que permiten reensamblar datos solo tras validación contextual, garantizando protección dinámica y mitigación avanzada de ataques laterales.


# 🛡️ GuardianIA: Sistema de Protección y Acceso Inteligente a Redes Fragmentadas

> Proyecto de ciberseguridad avanzada con inteligencia artificial como centinela de red, acceso por credenciales temporales, y reensamblaje condicional de datos.

## 📌 Descripción

A.N.G.E.L. — Autonomous Network Guardian with Encrypted Lobbying es una arquitectura innovadora de control y protección de redes, basada en la fragmentación dinámica de datos, lobbies virtuales segmentados y una inteligencia artificial encargada de custodiar, autorizar y ensamblar flujos de información. El sistema reemplaza los modelos tradicionales de cortafuegos y autenticación centralizada con un enfoque distribuido, adaptativo y consciente del comportamiento.

## 🔒 Características Clave

- 🧠 **Guardia IA Adaptativa**: supervisa eventos de red en tiempo real y controla accesos a los lobbies.
- 🧩 **Fragmentación Lógica de Red**: separa los datos y recursos en múltiples entornos virtuales.
- 🔐 **Acceso con Clave Temporal Encriptada (TCE)**: cada solicitud requiere una clave dinámica, generada por el mismo sistema IA.
- 🛠️ **Reensamblado Condicional**: los paquetes de datos solo se recomponen cuando el usuario/servicio presenta las credenciales correctas.
- 🕳️ **HoneyLobbies y Túneles Falsos**: zonas virtuales de distracción para mitigar y monitorear intrusiones.

## 🧬 Componentes

- `AI-Watcher`: motor central de IA que decide, aprende y reconfigura en tiempo real.
- `LobbyManager`: gestiona zonas virtuales, coordina flujos, activa lobbies según políticas dinámicas.
- `TCE-Generator`: algoritmo criptográfico efímero de claves únicas por sesión.
- `Reassembler`: servicio que recompone la información validada y autorizada.

## 📄 Documentación

- [`whitepaper.pdf`](./whitepaper.pdf): diseño técnico, filosofía del sistema, análisis de seguridad.
- [`patente_guardianIA.md`](./patente_guardianIA.md): borrador de patente técnica y reivindicaciones.

## 🚧 Estado del Proyecto

> `Etapa 1`: Arquitectura conceptual completada, definición de lógica de IA y protocolo de lobbies.  
> `Etapa 2`: Simulación de red e implementación de prototipo en entornos virtualizados (en curso).  
> `Etapa 3`: Validación técnica, documentación legal y roadmap hacia MVP (Q4 2025).

## 👨‍💻 Autor

**Lerry Alexander Elizondo Villalobos (LAEV)**  
Diseñador, arquitecto digital, estratega de sistemas descentralizados y fundador del Cartel de Bitcoiners.  
📧 laev.lab@proton.me | 📞 +50671148872  
🔗 [GitHub](https://github.com/lerryalexanderelizondo)

---

## ⚖️ Licencia

Este proyecto está protegido bajo una licencia de investigación cerrada. Cualquier uso, adaptación o distribución no autorizada será considerado violación de propiedad intelectual en trámite de patente.


Diagramas para la patente A.N.G.E.L.

1. Diagrama de Arquitectura General

Descripción:
Un esquema de alto nivel que muestra los principales componentes del sistema:

Usuarios / dispositivos solicitantes

AI Fragmentation Engine (motor de fragmentación IA)

Lobbys digitales segmentados (múltiples zonas aisladas)

Generador de Claves Temporales Cifradas

Módulo de Reensamblaje Condicional

Blockchain / Registro Inmutable

Mecanismo de Revocación y Auditoría


Objetivo:
Visualizar cómo fluye la solicitud de acceso, la fragmentación de la red, la generación y validación de claves, y el acceso condicional a datos.


---

2. Diagrama de Flujo de Operación

Descripción:
Flujo paso a paso de la interacción entre:

Inicio de la solicitud (usuario o dispositivo)

Evaluación contextual por IA (identidad, comportamiento, geolocalización)

Generación de clave temporal

Acceso a lobby digital

Reensamblaje de datos tras validación

Expiración y revocación automática


Objetivo:
Aclarar la secuencia lógica y temporal del proceso.


---

3. Diagrama de Fragmentación y Reensamblaje de Datos

Descripción:
Representación conceptual de cómo los datos o funciones se dividen en fragmentos aislados dentro de lobbys digitales y se reensamblan únicamente cuando se valida la clave temporal.

Objetivo:
Mostrar la estrategia anti-exfiltración y control granular.


---

Anexos Técnicos

A. Especificación Criptográfica

Algoritmos propuestos para la generación de claves temporales (ej. AES-256-GCM para cifrado simétrico, RSA-OAEP para clave pública).

Esquema de expiración y revocación de tokens.

Implementación posible de Zero-Knowledge Proofs para validación reforzada.


B. Modelos IA para Evaluación Contextual

Tipos de datos recolectados para contexto:

Identidad digital (firmas, wallets)

Comportamiento (análisis de patrones, frecuencia de acceso)

Geolocalización y dispositivo

Reputación y riesgo


Algoritmos ML sugeridos: clustering, redes neuronales, análisis de anomalías.


C. Arquitectura de Red y SDN

Descripción técnica de cómo usar SDN para crear lobbys virtuales.

Ejemplos de herramientas: Istio, Calico, Kubernetes Namespaces.

Mecanismos para aislamiento y microsegmentación.


D. Blockchain y Registro Inmutable

Uso de blockchain para auditoría: almacenamiento de logs de accesos, claves temporales y eventos.

Tecnologías posibles: Ethereum privada, Hyperledger Fabric, IPFS para almacenamiento distribuido.


Diagrama de Flujo de Operación — A.N.G.E.L.

Descripción paso a paso:

flowchart TD
    A[Inicio: Solicitud de acceso (usuario/dispositivo)] --> B[Ingreso a Lobby Digital]
    B --> C[IA Fragmentation Engine: Evalúa contexto]
    C --> D{¿Validación exitosa?}
    D -- Sí --> E[Genera Clave Temporal Cifrada]
    E --> F[Acceso Condicional a Fragmentos]
    F --> G[Reensamblaje de Datos/Servicios]
    G --> H[Operación dentro de permisos temporales]
    H --> I{¿Clave expirada o revocada?}
    I -- Sí --> J[Revocación de acceso y cierre de sesión]
    I -- No --> H
    D -- No --> K[Acceso denegado y monitoreo de evento]
    K --> L[Registro y alerta en blockchain / auditoría]
    J --> L


---

Explicación técnica:

1. Inicio: Un usuario o dispositivo realiza una solicitud para acceder a un recurso o servicio dentro de la red.


2. Ingreso a Lobby Digital: La solicitud es dirigida a un lobby virtual aislado, una microzona sin conexión directa con otros lobbys.


3. Evaluación Contextual IA: El motor de IA analiza múltiples factores del solicitante (firma digital, geolocalización, comportamiento histórico, reputación) usando modelos de ML para determinar riesgo y legitimidad.


4. Decisión de Validación:

Si la evaluación es exitosa, se procede a generar una clave temporal cifrada, única y con tiempo limitado.

Si falla, el acceso es denegado y el evento es registrado para análisis.



5. Generación de Clave Temporal: Un token criptográfico que solo funciona dentro de parámetros definidos (duración, ámbito, tipo de acceso).


6. Acceso Condicional: Se permite acceso restringido a los fragmentos específicos del recurso o servicio solicitado.


7. Reensamblaje: Los fragmentos aislados se recomponen en la capa lógica solo mientras la clave esté activa y validada.


8. Operación: El usuario opera dentro de los permisos temporales otorgados.


9. Expiración o Revocación: Cuando la clave expira o se revoca (por actividad sospechosa o finalización), el acceso se cierra inmediatamente.


10. Registro y Auditoría: Todos los eventos de acceso, generación y revocación de claves se registran en una blockchain o sistema inmutable para auditoría.



