---
ms.openlocfilehash: 95ea94c1f81a3b586d60d96dbd5a882dcdbe89fc
ms.sourcegitcommit: 47bd0e48c7dba1dde49baff60bc1eddc91ab10c5
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/05/2022
ms.locfileid: "145114185"
---
Puedes usar `defaults.run` para proporcionar las opciones `shell` y `working-directory` predeterminadas para todos los pasos de [`run`](/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepsrun) de un flujo de trabajo. También puedes establecer opciones predeterminadas para `run` que solo están disponibles para un trabajo. Para más información, vea [`jobs.<job_id>.defaults.run`](/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_iddefaultsrun). No puedes utilizar contextos o expresiones en esta palabra clave.

{% data reusables.actions.defaults-override %}

#### Ejemplo: Configurar el directorio de trabajo y shell predeterminados

```yaml
defaults:
  run:
    shell: bash
    working-directory: scripts
```
