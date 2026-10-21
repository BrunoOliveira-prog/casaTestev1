# casaTestev1

Visualizador 3D de planta de casa em Three.js. Cole uma planta em JSON (cômodos, paredes, portas e janelas) e veja o modelo em 3D.

- Vistas: perspectiva, isométrica e planta baixa
- Slider de corte de altura das paredes
- Rótulos com nome e área (m²) de cada cômodo
- Tema claro e escuro

## Como rodar

Abra o `index.html` no navegador. Precisa de internet para carregar o Three.js (jsDelivr) e as fontes (Google Fonts).

## Formato do JSON

- `walls[]`: `a` e `b` são pontos `[x, y]` em metros; `t` é a espessura; `openings[]` com `type` (`door`, `window`, `opening`), `at` (distância do ponto `a` até o centro), `w`, `h`, `sill`.
- `rooms[]`: `name`, `kind` (`social`, `servico`, `circulacao`, `intimo`, `umido`) e `pts` (cantos `[x, y]`).
