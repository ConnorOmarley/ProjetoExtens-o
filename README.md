# ProjetoExtens-o

Clone de interface da Netflix feito em **HTML, CSS e JavaScript puros**, como projeto acadêmico. Sem framework, sem build, sem dependência.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

## Telas

| Arquivo | O que é |
|---|---|
| `login.html` | Tela de entrada com e-mail e senha |
| `contas.html` | "Quem está assistindo?" — seleção de perfil |
| `index.html` | Tela inicial com banner de *Stranger Things*, busca e fileiras por categoria |
| `filmes.html` | Catálogo de filmes, banner de *Interestelar*, fileiras por gênero |
| `series.html` | Catálogo de séries, banner de *Breaking Bad*, fileiras por gênero |

O JavaScript está em um arquivo só, `ms.js`, com 64 bytes — a função `login()` só redireciona para `contas.html`. **A busca e a navegação entre fileiras não funcionam**; o filtro de pesquisa é a parte que ficou de fora.

Todo o layout é `style.css`, e `img/zgeTuV.jpg` é a única imagem do projeto.

## Rodar

Não tem build nem servidor. Só abra o `login.html` no navegador — ou, se preferir servir por HTTP:

```bash
python -m http.server 8000
```

## Limites conhecidos

- **A busca não filtra nada.** O `input` de pesquisa existe nas telas de filmes e séries, mas não tem listener ligado.
- **O login aceita qualquer coisa.** `login()` redireciona sem validar e-mail nem senha.
- **Não é responsivo.** O layout foi feito para tela grande e não tem breakpoint nem menu mobile.
- **As imagens são um único arquivo.** Os cards de catálogo usam cor e texto em vez de pôsteres.
- **Marca e conteúdo são da Netflix.** Projeto acadêmico, sem fins comerciais, sem vínculo com a Netflix.

## Licença

MIT
