En este apartado se presentan un conjunto de entidades de código con defectos identificadas. 
Para la identificación de defectos se utilizan herramientas específicas (InCode y PMD), herramientas de medición y valores umbrales (SourceMeter y RefactorIT) e inspecciones de código manual.

Por cada instancia del defecto identificada se debe crear una fila con la siguiente información:
C1: Nombre del defecto.
C2: Tipo de la entidad [subsistema|clase|método].
C3: Nombre único (cualificado) de la entidad anómala. Un mismo defecto puede involucrar varias entidades, una fila por cada una. 
C4: Rango de líneas de código donde aparece e hiperenlace al código fuente de la entidad del repositorio público  
C5: Conjunto de métricas e intervalos utilizados para su identificación si existen.
C6: Otras consultas aplicadas para la detección.

### Paquetes con defectos
|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |

### Clases con defectos


**Defectos dentro de clases- Medibles**

|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|
|            |           |             |          |                         |                         |

**Defectos dentro de clases- Complejidad innecesaria**

|     C1     |     C2    |     C3             |    C4    |          C5             |         C6              |
|------------|-----------|--------------------|----------|-------------------------|-------------------------|
| Andoni Vianez y Yobana Nido                                                                                |
| God class  | Clase     |Controller          | [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/controllers/Controller.java)   |   WMC ATFD TCC                     |  inCode y PMD           |
| God class  | Clase     |SelectionController | [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/controllers/SelectionController.java)   | WMC ATFD TCC                        |  inCode y PMD           |

**Defectos dentro de clases -  Duplicación**

|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|
| External Duplication | Método |  initListViewCourseModules(MainController mainController, Course actualCourse) | Rango de líneas de código: 71 – 168. [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/controllers/SelectionController.java) | N/A | inCode |
| External Duplication | Método |  initListViewCourseModules(Course actualCourse)| Rango de líneas de código: 71 – 168. [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/controllers/SelectionController.java) | N/A | inCode |
| Sibling Duplication | Método | createData(List<E> typeLogs, DataSet<E> dataSet) | Rango de líneas de código: 63 – 108. [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/multi/RankingTable.java) | N/A |  inCode |
|            |           |             |          |                         |                         |
| Andoni Vianez y Yobana Nido                                                                         |
| External Duplication | Método | SelectionController   | [Líneas ](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/controllers/SelectionController.java)| - | inCode |
| External Duplication | Método | SelectionCourseModuleControl   |[Líneas](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/controllers/SelectionCourseModuleController.java) | - | inCode |
| Sibling Duplication | Método | SigmaCourseAddressMap   | [Líneas](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/sigma/SigmaCourseAddressMap.java) | - | inCode |
| Sibling Duplication | Método | SigmaUsualAddressMap    | [Líneas](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/sigma/SigmaUsualAddressMap.java) | - | inCode |



**Defectos dentro de clases -  Lógica condicional**

|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |

**Defectos entre clases - Datos**

|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|
| Data Class | Clase     |     WebViewTabsController   |  Rango de líneas de código: 19 – 214. [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/controllers/WebViewTabsController.java)  |   WMC    |   inCode   |
| Data Clum  | Método    |   getUserCounts(…)     | Rango de líneas de código: 49 – 52. [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/model/datasets/DatasSetCourseModule.java)    |        NP       |    inCode    |
| Andoni Vianez y Yobana Nido  |     |        |     |               |       |
| Data Class  | Clase    | WebViewTabsController       |  [Clase](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/controllers/WebViewTabsController.java)    |  WOC, NOPA, NOAM, WMC             | inCode y PMD      |
| Data Class  | Clase    | DiscussionPost       | [Clase](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/model/DiscussionPost.java)    |  WOC, NOPA, NOAM, WMC             | inCode y PMD      |
| Data Clumps  | Clase    | DatasSet      | [Rango](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/model/datasets/DataSet.java)   |  -             | inCode    |
| Data Clumps  | Clase    | DatasSetCourseModule       |   [Rango](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/model/datasets/DatasSetCourseModule.java) |  -             | inCode      |

**Defectos entre clases – Herencia**

|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|
| Tradition Breaker | Clase | PointsTable | Rango de líneas de código: 37 – 320. [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/multi/PointsTable.java)  | N/A | inCode |
| Andoni Vianez y Yobana Nido           |           |             |          |                         |                         |
|       Tradition Breaker     |  Clase         |   RankingTable          |    [Clase](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/multi/RankingTable.java)     |       -                  |        inCode                 |
|            |           |             |          |                         |                         |

**Defectos entre clases – Responsabilidad**

|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|
| God Class  | Clase     |  Controller | Rango de líneas de código: 34 – 442. [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/controllers/Controller.java)   | WMC=64, ATFD=62, TCC=4.351%  |  Plugin PMD de Eclipse e inCode  |
| Message Chains | Método | createData(List<E> typeLogs, DataSet<E> dataSet)     | Rango de líneas de código: 101 – 140. [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/logs/TableLog.java) | CBO, RPC |  inCode  |
| Feature Envy | Método | exportCSV(String path)    |  Rango de líneas de código: 75 – 123. [Enlace](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/sigma/SigmaTableNotEnrolled.java) | CBO, RPC |  inCode  |
| Andoni Vianez y Yobana Nido             |
|     Feature Envy    |     Método   |     exportCSV      |   [Clase SigmaTableNotEnrolled](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/logs/TableLog.java)    |           CBO, LCOM              |         inCode              |
|     Feature Envy    |     Método   |     createData      |    [Clase SigmaTableNotEnrolled](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/logs/TableLog.java)    |           CBO, LCOM              |         inCode        |
|     Message Chains    |     Método   |     exportCSV      |    [Clase TableLog](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/logs/TableLog.java)    |           CBO, RPC              |         inCode          |
|     Message Chains    |     Método   |     createData      |    [Clase TableLog](https://github.com/yjx0003/UBUMonitor/blob/master/src/main/java/es/ubu/lsi/ubumonitor/view/chart/logs/TableLog.java)    |           CBO, RPC              |         inCode            |

**Defectos entre clases- Adecuación al cambio**

|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |

**Defectos entre clases- Biblioteca de clases**

|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |


### Métodos con defectos

|     C1     |     C2    |     C3      |    C4    |          C5             |         C6              |
|------------|-----------|-------------|----------|-------------------------|-------------------------|                       
|            |           |             |          |                         |                         |
|            |           |             |          |                         |                         |