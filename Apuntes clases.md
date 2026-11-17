# Metodología de presupuestación

La presupuestación de un proyecto de aprendizaje automático consiste en estimar los recursos necesarios para realizarlo. Entre ellos se incluyen el equipo de trabajo, el hardware, el tiempo de desarrollo, el almacenamiento de datos y la capacidad de procesamiento.

## Modelo de presupuestación de Merlino

El presupuesto inicial debe considerarse una estimación y no un valor definitivo. Puede modificarse debido a imprevistos, cambios en el alcance o variaciones en los recursos necesarios.

Un presupuesto demasiado alto puede hacer que el cliente rechace la propuesta, mientras que uno demasiado bajo puede generar pérdidas para la empresa. Por este motivo, es importante justificar la estimación mediante:

- El alcance del proyecto.
- El tiempo requerido.
- Los algoritmos y las tecnologías previstos.
- El equipo necesario.
- Las fechas tentativas de inicio y finalización.

La formulación del proyecto incluye una descripción de la idea general, una estimación de tiempos, los algoritmos que podrían utilizarse y un equipo de trabajo tentativo. Por ejemplo, se puede establecer que, si el proyecto comienza el 1 de septiembre, finalizará el 30 de septiembre. Luego, es necesario coordinar la disponibilidad de las personas involucradas para que dediquen el tiempo previsto.

Una vez elaborada la formulación, se presenta el presupuesto al empleador, quien puede aceptarlo o rechazarlo. El valor debe ser realista: si es demasiado alto, puede no ser aprobado; si es demasiado bajo, puede producir pérdidas.

La estimación del presupuesto es uno de los aspectos más difíciles de la ciencia de datos, porque debe contemplar tanto los recursos conocidos como los posibles imprevistos.

## Costos de un proyecto

Los principales costos de un proyecto de aprendizaje automático son:

- **Costo del equipo:** sueldos y dedicación de las personas involucradas.
- **Costo de almacenamiento:** espacio necesario para guardar los datos, modelos y resultados.
- **Costo de procesamiento:** recursos necesarios para entrenar, evaluar y ejecutar los modelos.

![Principales costos de un proyecto de aprendizaje automático](https://github.com/user-attachments/assets/3ad83533-bc63-4c20-a634-ba1650f24274)

## FinOps: comparación entre entornos

FinOps es una disciplina que busca relacionar las decisiones financieras con el uso de recursos tecnológicos. Permite controlar, analizar y optimizar los costos de infraestructura, especialmente en entornos de computación en la nube.

| Componente de costo | Entorno on-premises | Entorno en la nube |
|---|---|---|
| **CapEx inicial** | Alto: requiere comprar servidores, GPU, almacenamiento e infraestructura física. | Bajo o nulo: se utiliza un modelo de pago por uso, sin inversión inicial en hardware. |
| **OpEx recurrente** | Bajo y predecible, aunque incluye energía, refrigeración y mantenimiento. | Variable y potencialmente alto, debido al uso de recursos, la transferencia de datos y los servicios administrados. |
| **Escalabilidad** | Compleja y costosa: requiere inversiones adicionales en hardware y tiempo de instalación. | Flexible y bajo demanda, con aprovisionamiento rápido y escalabilidad automática. |
| **Costos ocultos** | Personal de TI, redundancia y recuperación ante desastres. | Transferencia de datos (*data egress*), servicios administrados y sobreaprovisionamiento. |
| **Control y personalización** | Mayor control sobre el hardware, la seguridad y la privacidad de los datos. | Menor control directo y posible dependencia del proveedor (*vendor lock-in*). |

La elección entre una solución on-premises y una solución en la nube depende principalmente del patrón de uso de la carga de trabajo. Los proyectos de investigación y desarrollo, o aquellos con cargas intermitentes y experimentales, pueden beneficiarse de la flexibilidad de la nube. En cambio, las cargas de trabajo sostenidas y predecibles pueden justificar una infraestructura propia.

## Optimización del uso de recursos
El objetivo de la optimización de uso es reducir la cantidad de recursos consumidos sin afectar los resultados del proyecto. Algunas estrategias son:

- **Right-sizing:** ajustar el tamaño de las instancias de cómputo para que coincidan con los requisitos reales de la carga de trabajo.
- **Particionamiento de GPU:** utilizar tecnologías como NVIDIA Multi-Instance GPU (MIG) para dividir una GPU física en unidades más pequeñas. Esto permite aprovechar mejor el hardware cuando un modelo no necesita utilizar la GPU completa.
- **Optimización del modelo:** aplicar compresión de modelos y otras técnicas a nivel de código para reducir el consumo de recursos durante el entrenamiento y la inferencia.
- **Refinamiento de prompts:** reducir la cantidad de tokens utilizados y diseñar instrucciones más precisas.
- **Control de bucles infinitos:** monitorear las aplicaciones para evitar ejecuciones innecesarias que aumenten los costos de inferencia y entrenamiento.

## Modelo de madurez de inteligencia artificial
<img width="1398" height="712" alt="image" src="https://github.com/user-attachments/assets/2697bc10-0397-4a69-b413-67ffad5f6be2" />

El modelo de madurez de IA presentado organiza a las organizaciones en cinco niveles, según el grado de adopción e integración de la inteligencia artificial:

1. **Nivel 1 — Conciencia (*Awareness*):** existe un interés inicial por la IA, aunque puede haber expectativas exageradas o riesgo de sobrevaloración (*overhyping*).
2. **Nivel 2 — Activo (*Active*):** la organización experimenta con IA, principalmente en el contexto de proyectos de ciencia de datos.
3. **Nivel 3 — Operacional (*Operational*):** la IA se utiliza en producción y genera valor, por ejemplo, mediante la optimización de procesos o la innovación de productos y servicios.
4. **Nivel 4 — Sistémico (*Systemic*):** la IA se utiliza de forma generalizada para transformar procesos digitales y cadenas de valor, además de habilitar nuevos modelos de negocio digitales.
5. **Nivel 5 — Transformacional (*Transformational*):** la IA forma parte de la estrategia y del funcionamiento central de la organización; constituye parte de su identidad empresarial.

## Participantes en el ciclo de vida del aprendizaje automático

- **Analista de aprendizaje automático:** analiza el problema y estudia la viabilidad de la solución.
- **Ingeniero de datos:** diseña, construye y mantiene los sistemas de almacenamiento y procesamiento de datos.
- **Científico de datos:** explora los datos, desarrolla modelos y evalúa sus resultados.
- **Ingeniero de MLOps:** automatiza y mantiene los procesos de entrenamiento, despliegue, monitoreo y actualización de los modelos.
