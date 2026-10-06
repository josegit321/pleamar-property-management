# Cómo contribuir

Gracias por ayudar a mejorar Pleamar.

## Flujo recomendado

1. Abre un issue para describir el problema o la mejora propuesta.
2. Crea un fork del repositorio si no tienes acceso directo como colaborador.
3. Crea una rama desde `main`:

   ```bash
   git switch -c mejora/nombre-breve
   ```

4. Realiza cambios pequeños y enfocados.
5. Comprueba el sitio en escritorio y en una pantalla móvil.
6. Verifica los idiomas español e inglés y la navegación por teclado.
7. Crea commits descriptivos:

   ```bash
   git add .
   git commit -m "Mejora la navegación móvil"
   ```

8. Publica tu rama y abre un pull request hacia `main`.

## Antes de abrir el pull request

- El sitio carga sin errores en la consola del navegador.
- Las imágenes tienen texto alternativo adecuado.
- Los cambios funcionan a 320 px de ancho o más.
- El contraste y el foco visible se mantienen.
- No se inventan cifras comerciales, testimonios ni resultados.
- Las nuevas imágenes están optimizadas y tienen permiso de uso.
- El pull request explica qué cambia, por qué y cómo se verificó.

## Criterios de diseño y producto

`PRODUCT.md` define la audiencia y el objetivo del sitio. `DESIGN.md` contiene las reglas visuales. Si una propuesta cambia esas decisiones, descríbela claramente en el issue antes de implementarla.

## Formas de participar sin programar

También puedes aportar creando issues con correcciones de texto, traducciones, problemas de accesibilidad, observaciones desde móvil o sugerencias sobre el proceso para propietarios.

