# Definição de Pronto — Viveiro

> Documento herdado. Última alteração: 2026-04-11.

## Definição geral

Uma história está pronta quando:

- todos os critérios de aceitação definidos para a história foram atendidos;
- a funcionalidade foi implementada e testada;
- não existem erros conhecidos que impeçam o funcionamento da história;
- o resultado corresponde ao que foi definido no `BACKLOG.md`;
- a equipe verificou os critérios de aceitação;
- o cliente aprovou a entrega.

---

## Critérios de aceitação

Os critérios abaixo correspondem às histórias registradas no `BACKLOG.md`.

### V-01 — Página da pessoa

A história está pronta quando:

- clicar no nome do autor em qualquer cartão abre a página da pessoa;
- a página exibe nome, tipo (aluno ou professor), curso e interesses;
- a página apresenta as ideias publicadas pela pessoa;
- o título de cada ideia publicada pode ser clicado;
- quando a pessoa não possui ideias publicadas, aparece a mensagem "ainda não publicou ideias";
- existe uma forma de retornar ao mural sem utilizar o botão de voltar do navegador.

---

### V-02 — Filtro por curso

A história está pronta quando:

- é possível selecionar um curso como filtro;
- ao selecionar um curso, apenas as ideias relacionadas ao curso selecionado são exibidas;
- quando nenhum filtro é selecionado, todos os projetos de pesquisa são exibidos;
- os filtros ficam disponíveis junto à área de pesquisa;
- é possível remover o filtro e retornar à lista completa.

---

### V-03 — Publicar uma ideia

A história está pronta quando:

- existe um formulário contendo título, resumo e tags;
- o usuário consegue enviar uma nova ideia;
- a ideia publicada aparece no topo do mural sem necessidade de recarregar a página;
- a ideia registra corretamente o autor e a data;
- o envio é impedido quando o título estiver vazio;
- uma mensagem informa ao usuário o que precisa ser preenchido;
- a contagem total de ideias do mural é atualizada após a publicação;
- não é permitido cadastrar títulos duplicados;
- o resumo respeita o limite de tamanho definido para o sistema.

---

### V-04 — Encontrar ideias que combinam comigo

A história está pronta quando:

- existe um campo de busca por palavras-chave;
- o usuário consegue pesquisar ideias utilizando palavras-chave;
- os filtros podem ser utilizados junto com a pesquisa por palavras-chave;
- os resultados da busca correspondem aos termos pesquisados;
- a pesquisa apresenta os resultados sem demora que impeça sua utilização;
- quando não existem resultados, o sistema informa que nenhuma ideia foi encontrada.

---

### V-05 — Entrar e sair de um grupo

A história está pronta quando:

- a lista de grupos informa se o usuário está dentro ou fora de cada grupo;
- o usuário consegue entrar em um grupo;
- ao entrar, seu nome é acrescentado à lista de membros;
- o contador de membros é atualizado após a entrada;
- o usuário consegue sair de um grupo;
- ao sair, seu nome é removido da lista de membros;
- o contador de membros é atualizado após a saída;
- a lista apresenta os nomes dos membros;
- a troca da pessoa em "navegando como" atualiza corretamente seus grupos;
- o usuário recebe uma confirmação ao entrar ou sair de um grupo.

---

### V-06 — Estados da ideia

A história está pronta quando:

- cada projeto de pesquisa possui um estado;
- os estados disponíveis são "semente", "germinando" e "proposta";
- o estado atual da ideia pode ser identificado pelo usuário;
- apenas usuários autorizados conseguem alterar o estado;
- a alteração do estado fica registrada corretamente.

---

### V-07 — Registrar interesse em participar

A história está pronta quando:

- cada ideia possui o controle "tenho interesse em participar";
- o usuário consegue registrar seu interesse;
- após registrar o interesse, seu nome aparece na lista de interessados;
- a mesma pessoa não consegue registrar interesse duas vezes na mesma ideia;
- o usuário consegue desfazer seu interesse;
- ao desfazer o interesse, seu nome é removido da lista;
- o número de interessados exibido no cartão corresponde à quantidade de pessoas na lista;
- o autor da ideia consegue visualizar a lista completa de interessados.

---

### V-08 — Não perder o que foi escrito

A história está pronta quando:

- os dados preenchidos pelo usuário são salvos durante a edição;
- os dados salvos permanecem disponíveis após o fechamento ou recarregamento da página;
- ao carregar novamente a página, os dados salvos são recuperados automaticamente;
- os dados recuperados correspondem ao que havia sido preenchido anteriormente.

---

### V-09 — Aviso de novo interessado

A história está pronta quando:

- ao registrar interesse em uma ideia, o autor recebe uma notificação;
- a notificação é enviada em até um minuto após o registro do interesse;
- a notificação apresenta o nome de quem demonstrou interesse;
- a notificação apresenta o título da ideia correspondente;
- ao tocar na notificação, o usuário é direcionado para a ideia correspondente.

---

### V-10 — Ideias paradas

A história está pronta quando:

- ideias que não possuem atualizações por mais de 30 dias são identificadas;
- as ideias paradas possuem um indicador visual;
- é possível visualizar uma lista contendo somente as ideias paradas;
- quando uma ideia recebe nova atividade, ela deixa de ser considerada parada;
- o indicador de ideia parada é atualizado corretamente após uma nova atividade.

---

### V-11 — Relatório por curso

A história está pronta quando:

- existe um relatório das ideias organizadas por curso;
- o relatório apresenta a quantidade de ideias por curso;
- o relatório apresenta o número de alunos participantes;
- o relatório apresenta a quantidade de projetos em cada estado;
- é possível selecionar um curso específico para visualizar seus dados;
- as informações apresentadas no relatório correspondem aos dados registrados no sistema.

---

### V-12 — Exportar / importar o estado

A história está pronta quando:

- o administrador consegue exportar os dados do sistema;
- os dados podem ser exportados em arquivo JSON;
- o administrador consegue importar um arquivo previamente exportado;
- os dados do arquivo importado são carregados corretamente;
- os dados existentes são atualizados de acordo com o arquivo importado;
- arquivos inválidos são identificados;
- quando um arquivo inválido é selecionado, o sistema apresenta uma mensagem de erro;
- uma exportação seguida de uma importação mantém os dados corretamente.

---

## Defeitos conhecidos

Os defeitos registrados no `BACKLOG.md` também devem ser verificados quando suas respectivas funcionalidades forem trabalhadas:

- **B-01** — a busca deve reconhecer termos independentemente de diferenças entre letras maiúsculas, minúsculas e acentuação;
- **B-02** — o número de apoios deve ser atualizado imediatamente após uma alteração;
- **B-03** — deve ser possível remover um filtro aplicado por uma tag sem recarregar a página;
- **B-04** — quando uma busca não encontrar resultados, o mural deve apresentar uma mensagem informando a situação;
- **B-05** — títulos compridos não devem ultrapassar os limites dos cartões ou sobrepor outros cartões;
- **B-06** — as datas devem ser exibidas no formato `DD/MM/AAAA`.

---

## Verificação da Definição de Pronto

Antes de mover uma história para a coluna **Concluído** no `PLANO.md`, a equipe deve verificar:

- [ ] todos os critérios de aceitação da história foram atendidos;
- [ ] a funcionalidade foi testada;
- [ ] os defeitos que impedem o funcionamento da história foram corrigidos;
- [ ] a implementação corresponde ao que está registrado no `BACKLOG.md`;
- [ ] a equipe verificou o resultado;
- [ ] o cliente aprovou a história.

Uma história somente deve ser registrada como **Concluída** no quadro quando todos os critérios aplicáveis tiverem sido verificados.
