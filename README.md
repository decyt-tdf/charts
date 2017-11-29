# Rharts
Mono-repo de todos los charts que desarrollamos.

Este repositorio es utilizado tanto para el desarrollo como como repositorio helm.
El branch master contiene únicamente documentación.
Los charts considerados maduros se encuentran en el branch stable.
Los charts que no han superado aún el proceso de incubación se encuentran en el branch incubator.

## Uso

### Repositorio estable

```
  $ helm repo add decytStable 'https://raw.githubusercontent.com/decyt-tdf/charts/stable/'
  $ helm repo update
  $ helm install --name nombreDeRelease decytStable/nombreDelChart
```

### Repositorio incubadora

```
  $ helm repo add decytIncubator 'https://raw.githubusercontent.com/decyt-tdf/charts/incubator/'
  $ helm repo update
  $ helm install --name nombreDeRelease decytStable/nombreDelChart
```

### Criterio

Los charts se graduan de la incubadora cuando cumplen con una serie de requisitos de calidad y documentación.
Buena parte del funcionamiento del repositorio, así como del criterio de graduación están basados en el repositorio oficial de charts de kubernetes.

### WIP

Este es un trabajo en progreso. Todavía resta documentar el criterio de graduación, crear pull request templates e issue templates, describir el proceso de colaboración y brindar plantillas que permitan inicializar charts con una base más completa y acorde a nuestro caso que los generados por `helm generate`.

Falta mucho por hacer pero nos movemos rápido. No pierdas de vista este repositorio por muchos días.
