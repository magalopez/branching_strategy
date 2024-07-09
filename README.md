# branching_strategy

Manteniendo el flujo de trabajo actual con algunas modificaciones, enfocándose en las HU que requieren mantenerse en el ambiente de test por un tiempo prolongado.

1. Desarrollo en ramas feature: Se crean a partir de develop.
2. Pull Request y ambiente dinámico:
    - Al crear PR de feature a develop, se genera un ambiente dinámico.
    - QA realiza pruebas en este ambiente.
3. Merge a develop:
    - Tras la aprobación de QA, se hace merge squash a develop.
    - Develop sirve como ambiente de test para pruebas integradas.