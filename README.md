# Ciencia-de-datos

Este repositorio contendrá las actualizaciones de nuestra interfaz
```mermaid
flowchart TD
    A[YOLO-NAS: Object detection] --> B[Estimation of position and orientation]
    B --> C{Valid position?}
    C -- Yes --> D[Send coordinates to YuMi via EGM]
    D --> E[Movement of the ABB YuMi robot]
    E --> F[Gripper activation via RWS]
    F --> G[Sample/object manipulation]
    C -- No --> H[Notify error/handle exception]
```
