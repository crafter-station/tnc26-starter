# Contexto para agentes

Este fichero lo leen Claude Code, Cursor, Codex y cualquier otro agente que trabaje en
este repositorio. Dice en qué situación estás para que no propongas lo que se propone
en un proyecto normal.

## La situación

Esto es un hackathon de **12 horas**. Un equipo de 3 a 5 personas, un solo día, y una
demo **en vivo de 3 minutos** delante de un jurado a las 20:15. El código se congela a
las 20:00.

Lo que se juzga es lo que ocurre en esos 3 minutos. No la cobertura de tests, ni la
arquitectura, ni lo bien tipado que esté.

## Cómo priorizar

1. **El camino feliz primero, y entero.** Vale más un flujo que funciona de principio
   a fin que cinco features a medias. Si algo no se ve en la demo, no existe.
2. **Elige lo aburrido.** La librería que el equipo ya conoce gana a la que es mejor.
   No es el día de aprender una herramienta nueva.
3. **Despliega temprano.** Pon algo en producción en la primera hora, aunque sea un
   «hola mundo». Descubrir el deploy a las 19:00 es cómo se pierden los hackathons.
4. **No refactorices.** Si funciona y es feo, funciona. Solo se toca lo que bloquea.
5. **Datos de verdad, aunque sean pocos.** Una demo con tres registros reales convence
   más que una con mil generados.

## Reglas prácticas

- **Commits pequeños y frecuentes**, y empuja a `main` a menudo. El equipo entero
  trabaja sobre este repo y el que se queda tres horas sin empujar bloquea a los demás.
- **`main` siempre arrancable.** Si rompes el arranque, arréglalo o revierte antes de
  seguir con otra cosa.
- **El repositorio es público.** Nunca escribas claves, tokens ni credenciales en el
  código ni en los commits. Van a un `.env` local, que ya está ignorado. Si se te
  escapa una, avisa al equipo: rotarla es más rápido que limpiar la historia.
- **Mantén el README del proyecto al día** con cómo arrancarlo en dos comandos. El
  jurado y los mentores van a intentarlo.

## Antes de las 20:00

- [ ] `main` arranca desde cero siguiendo el README
- [ ] La demo está desplegada y accesible desde una URL
- [ ] No hay secretos en el repositorio
- [ ] El pitch de una frase está escrito y entregado en el dashboard
- [ ] Alguien ha ensayado los 3 minutos, cronómetro en mano

## Qué NO hacer

- Reescribir algo que ya funciona porque «así queda mejor».
- Añadir autenticación, panel de admin o multi-idioma si la demo no lo necesita.
- Empezar una migración de framework después del mediodía.
- Dejar el despliegue para el final.
