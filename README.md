# DEM — Didática do Estudo do Meio

Projeto de apoio didático para a unidade de **Didática do Estudo do Meio**, com módulos interativos e atividades experimentais para uso em contexto de formação e sala de aula.

Publicação (GitHub Pages): [https://jota187.github.io/DEM/](https://jota187.github.io/DEM/)

## Estrutura do projeto

```text
DEM/
├── index.html                    # Página inicial (hub com navegação por temas)
├── README.md
├── assets/
│   ├── css/
│   │   └── shared.css            # Estilos partilhados entre páginas
│   └── icons/
│       ├── favicon_bayes.png
│       └── favicon_medir.png
├── bayes/
│   └── teorema_bayes.html        # Módulo Teorema de Bayes
├── medir/
│   └── aprender_medir.html       # Módulo Aprender a Medir
└── experimenta/                  # Submodule com atividades experimentais
```

## Módulos disponíveis

- **Bayes**: módulo interativo sobre probabilidade condicional, atualização de crenças e aplicações pedagógicas.
- **Medir**: módulo sobre medição em Física, precisão/exatidão, erros e incerteza.
- **Experimenta**: conjunto de atividades experimentais (abertas e fechadas) por tema.

## Como correr localmente

Como são páginas estáticas, podes abrir diretamente o `index.html` no browser.  
Para evitar problemas de caminhos e testar de forma mais próxima do GitHub Pages, recomenda-se usar um servidor local:

### Opção 1: VS Code / Cursor Live Server

1. Abrir a pasta do projeto.
2. Executar **Open with Live Server** sobre `index.html`.
3. Aceder ao URL local indicado (ex.: `http://127.0.0.1:5500`).

### Opção 2: Python

Na raiz do projeto:

```bash
python -m http.server 8000
```

Depois abrir:

```text
http://localhost:8000/
```

## Nota sobre o submodule `experimenta`

Se a pasta `experimenta` aparecer vazia, o submodule não está inicializado.  
Executar na raiz do projeto:

```bash
git submodule update --init --recursive
```
