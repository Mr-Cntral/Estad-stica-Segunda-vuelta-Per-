# Dashboard Segunda vuelta Perú 2026

Sube estos archivos a la raíz del repositorio:

- `index.html`
- `data.json`

También deben estar en la raíz las imágenes:

- `KeykoFujimori version oscuro.png`
- `KeykoFujimori.png`
- `Logo del partido Fuerza Popular.svg`
- `Logo del partido Juntos por el Peru.svg` o `Logo del partido Juntos por el Peru.png`
- `RobertoSanchez version oscuro.png`
- `RobertoSanchez.png`

## Cómo actualizar los números

Solo edita `data.json`.

Campos principales:

- `updatedAtLabel`: hora del corte.
- `current.actasPct`: porcentaje de actas contabilizadas.
- `current.countedActas`: actas contabilizadas.
- `current.pendingActas`: actas pendientes.
- `current.validVotes`: votos válidos contabilizados.
- `candidates.roberto.votes`: votos de Roberto.
- `candidates.roberto.percent`: porcentaje de Roberto.
- `candidates.keiko.votes`: votos de Keiko.
- `candidates.keiko.percent`: porcentaje de Keiko.
- `foreign`: datos del extranjero.
- `timeline`: cortes históricos para la línea del gráfico.

## Sobre el logo JP

Si el archivo real es SVG, usa:

```json
"logoPaths": [
  "Logo del partido Juntos por el Peru.svg",
  "Logo del partido Juntos por el Peru.png"
]
```

El HTML probará primero SVG y si falla intentará PNG.
