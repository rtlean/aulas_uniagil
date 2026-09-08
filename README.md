# Gestão de Projetos com IA — Uniagil

App responsivo de apoio à disciplina de pós-graduação ministrada por Roberto Trintin: 12 horas em quatro encontros online.

## Conteúdo

1. Enquadramento, valor e contexto confiável.
2. Escopo, abordagem, prazo e custo.
3. Desempenho, riscos e controle de mudanças.
4. Comunicação, rotinas com IA e benefícios.

Cada encontro possui conteúdo, prática guiada, prompt, campos de resposta, checklist, autoavaliação e materiais para download. O caso integrador Fluxo Claro usa dados fictícios.

## Executar localmente

Requer Python 3 apenas para servir os arquivos; não há instalação de dependências.

```bash
python -m http.server 8000 --directory dist
```

Abra http://localhost:8000 no navegador.

## Estrutura

- `dist/index.html`: estrutura da página.
- `dist/style.css`: layout responsivo e estilos.
- `dist/content.js`: conteúdo dos encontros, caso didático e CSV.
- `dist/app.js`: navegação, formulários, exportação e autoavaliação.
- `.openai/hosting.json`: identificação do Site existente e diretório de publicação.

Os arquivos de `dist/` são o código-fonte editável deste projeto estático. Não são gerados por compilação.

## Editar

Altere aulas, prompts, campos e exercícios em `dist/content.js`. Edite `dist/app.js` para mudar interações e `dist/style.css` para mudar o visual. Valide a sintaxe, se Node.js estiver disponível:

```bash
node --check dist/content.js
node --check dist/app.js
```

## Publicação

Qualquer hospedagem estática pode servir `dist/`. A publicação existente está em:
https://gestao-projetos-ia-rtlean.rtrintin.chatgpt.site

Na entrega inicial, o Site está restrito ao proprietário. O repositório GitHub é público, mas isso não muda o acesso do Site. Este repositório não possui implantação automática configurada. Atualizar o GitHub não atualiza automaticamente a publicação existente.

O manifesto de Sites identifica a publicação original; não o reutilize para criar um Site independente.

## Limites da versão

- Respostas ficam apenas na memória da aba; fechar ou recarregar apaga os campos. Baixe as respostas ao terminar.
- Não há cadastro de alunos, persistência em servidor, correção por IA ou envio de atividades ao professor.
- Os prompts são executados pelo aluno em sua própria conta ChatGPT ou Claude.
- Não há sincronização automática com o Notion.
- Esta cópia pública não inclui links internos do Notion.
- A tipografia usa Google Fonts, com fontes alternativas quando indisponível.
- Dados do caso são sintéticos, não representam uma organização real.
