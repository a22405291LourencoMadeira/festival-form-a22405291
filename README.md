# festival

## Alterações e Correções

`festival/models.py`
- Adicionado o campo `acessibilidade_mobilidade_reduzida` à classe `Palco`.

`festival/forms.py`
- `ConcertoForm` atualizado para incluir todos os campos: banda, dia, hora e palco.
- `PalcoForm` atualizado para incluir o novo campo `acessibilidade_mobilidade_reduzida`.

`festival/urls.py`
- Adicionada rota para apagar concerto.
- Adicionada rota para criar concerto.
- Adicionada rota para editar palco.

`festival/views.py`
- `dias_view` corrigida para ordenar os dias crescentemente.
- Adicionada `apagar_concerto_view`.
- Adicionada `criar_concerto_view`.
- Adicionada `editar_palco_view`.

`templates/festival/layout.html`
- Corrigido o link "Criar concerto" que estava vazio.

`templates/festival/concerto.html`
- Adicionado botão "Apagar concerto" com form POST.

`templates/festival/palcos.html`
- Corrigido o link "Editar palco" que estava vazio.
- Adicionada capacidade, número de concertos e ícone de acessibilidade por palco.

`templates/festival/criar_concerto.html`
- Criado o template em falta para a página de criar concerto.