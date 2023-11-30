[Documentation](https://expressjs.com/es/starter/installing.html).

#### Arquitectura de proyecto Node

```
src
│   index.js        # Entry point for application
└───config          # Application environment variables and secrets
└───controllers     # Express controllers for routes, respond to client requests, call services
└───loaders         # Handles all startup processes
└───middlewares     # Operations that check or maniuplate request prior to controller utilizing
└───models          # Database models
└───routes          # Express routes that define API structure
└───services        # Encapsulates all business logic
└───test            # Tests go here
```

**Notas:** Siempre se sugiere usar constantes en sus proyectos, en casos como:

1. Si la constante es un valor fijo para comparar (if) o mostrar en pantalla
   debe ir en mayuscula.
   MXN, USD, PI, MAX_SIZE
2. Si la constante guarda un valor logico q se utiliza pero no muta ni trampoco
   es visible o comparable se debe declarar en minuscula.
   port
