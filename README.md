# 🎲 BackgammonBase

Suite de backgammon en **un único archivo HTML**: tablero, partidas y matches, motor propio, análisis con informe, decisiones de cubo, aperturas, carrera y entrenador. Hermana de [AjedrezBase](https://github.com/rkarillo-tech/ajedrezbase).

**Versión web:** https://rkarillo-tech.github.io/backgammonbase/ (instalable y sin conexión)

## Qué hace

- **Tablero** con arrastre o clic, todas las reglas (uso obligatorio de dados, dado mayor, barra, golpes, sacar), dados automáticos o manuales y cubo de doblaje.
- **Partidas sueltas y matches** a 1-11 puntos con regla de Crawford, gammons y backgammons.
- **Motor heurístico propio** (pips, puntos, bloqueos, anclas, tiros exactos, barra) a 1 o 2 jugadas, más **tablas exactas de retirada** (54 264 posiciones por bando, calculadas en el navegador).
- **Análisis de la partida**: equity perdida por jugada y por decisión de cubo (modelo de Janowski), símbolos ?! ? ??, comentarios en español, PR aproximado, momentos clave y qué practicar. **Aprende de tus errores** con los mismos dados.
- **Variantes y comentarios**, planilla de dos columnas o lista, gráfico de probabilidad.
- **Formatos**: `.mat` (Jellyfish / GNU Backgammon), **XGID** (eXtreme Gammon), **Position ID** (GNU BG) y JSON completo.
- **Biblioteca** local (IndexedDB) con favoritas, etiquetas, marcadores, búsqueda en comentarios y copia de seguridad.
- **Entrenar**: tarjetas con repetición espaciada, las 15 tiradas de apertura y:
  - **🧮 Contar casillas**: se marca una ficha y sale un dado; pulsas el punto donde cae. Niveles: un dado, los dos dados seguidos, entrar desde la barra, sacar fichas, fichas del rival y mezcla. Si fallas, el tablero numera el recorrido casilla a casilla. Opción «sin números» para contar de memoria.
  - **🔢 Recuento de pips** en cinco niveles: un montón (fichas × punto), un cuadrante, un bando, los dos bandos y conteo continuo tras una jugada. Al corregir, el tablero muestra los pips de cada montón y la cuenta desglosada.
  - **📖 Lecciones con diagramas**: cómo se cuentan las casillas (numeración, barra, sacar fichas, distancias de golpe) y cómo se cuentan los pips (multiplicar, cuadrantes, cancelar, conteo continuo).
- **Ayuda al mover**: al pulsar una ficha, cada destino indica con qué dado llega («4», «6+4», «3×3»).
- Jugar contra la **CPU** (8 niveles), imagen PNG, impresión/PDF y enlaces para compartir.

## Uso

Abre `index.html` en Chrome, Edge o Firefox (doble clic) o usa la versión web. No necesita conexión ni descarga nada de terceros.

## Limitaciones

El motor es heurístico, sin red neuronal: sirve para jugar y estudiar, pero no tiene la fuerza de GNU Backgammon o XG. Las decisiones de cubo son de dinero (en matches, aproximadas).

## Licencia

MIT © 2026 Rafael Karino Arillo ([rkarillo-tech](https://github.com/rkarillo-tech)). Ver [LICENSE](LICENSE).
