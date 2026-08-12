# Backlog do Viveiro

> Documento herdado. Escrito ao longo do 1º semestre de 2026 pela equipe anterior.
>
> **Última alteração:** 2026-08-24.
>
> **Aviso de quem escreveu:** algumas destas histórias passaram pela revisão do cliente e outras não. Não me lembro quais. Boa sorte. — **R.M.**

---

# Histórias escritas

## V-01 — Página da pessoa

**Como** aluno que encontrou uma ideia interessante,

**quero** ver a página de quem a publicou,

**para** saber se temos interesses em comum antes de procurá-la.

### Pronto quando

- clicar no nome do autor, em qualquer cartão, abre a página dessa pessoa;
- a página mostra nome, tipo (aluno ou professor), curso e interesses;
- a página lista as ideias publicadas por essa pessoa, com o título clicável;
- se a pessoa não publicou nenhuma ideia, aparece a frase **"ainda não publicou ideias"** no lugar da lista vazia;
- existe um caminho de volta ao mural sem usar o botão do navegador.

---

## V-02 — Filtro por curso

**Como** aluno que quer encontrar uma ideia interessante,

**quero** filtrar as ideias por curso,

**para** encontrar ideias relacionadas ao meu curso.

### Pronto quando

- ao selecionar um curso, apenas ideias daquele curso são exibidas;
- quando filtros não forem selecionados aparecem todos os projetos de pesquisa;
- os filtros ficam disponíveis ao lado da barra de pesquisa;
- ao clicar em um filtro na pesquisa é possível voltar para tela inicial.

---

## V-03 — Publicar uma ideia

**Como** aluno com uma ideia na cabeça,

**quero** publicá-la sem depender de ninguém,

**para** que ela exista antes de eu esquecer.

### Pronto quando

- existe um formulário com título, resumo e tags;
- ao enviar, a ideia aparece no topo do mural imediatamente, sem recarregar a página;
- a ideia criada traz, como autor, o nome de quem está navegando, e a data de hoje;
- título vazio impede o envio e mostra uma mensagem dizendo o que falta;
- a contagem total de ideias exibida no mural aumenta em um;
- não permitir títulos duplicados;
- existir limite para o tamanho do resumo.

---

## V-04 — Encontrar ideias que combinam comigo

**Como** visitante do mural,

**quero** encontrar rapidamente as ideias que combinam comigo,

**para** não perder tempo.

### Pronto quando

- existir um campo de busca por palavras-chave;
- os filtros podem ser utilizados junto com a pesquisa por palavras-chave;
- a busca for rápida;
- o resultado for relevante.

---

## V-05 — Entrar e sair de um grupo

**Como** aluno que quer se aproximar de um tema,

**quero** entrar num grupo,

**para** acompanhar o que se discute ali.

### Pronto quando

- a lista de grupos mostra, em cada grupo, se estou dentro ou fora;
- entrar acrescenta meu nome à lista de membros e o contador sobe;
- sair remove meu nome e o contador desce;
- a lista mostra os nomes dos membros, não apenas o número;
- trocar a pessoa em "navegando como" muda corretamente o que aparece como "meus grupos";
- o usuário recebe confirmação ao entrar ou sair do grupo.

---

## V-06 — Estados da ideia

**Como** usuário,

**quero** que as ideias tenham estados,

**para** que seja possível distinguir uma ideia entre uma ideia em fase inicial e uma em fase final.

### Pronto quando

- os estados estiverem implementados em cada projeto de pesquisa;
- apenas usuários autorizados podem alterar o estado.

> **Obs.:** falamos em três estados — semente, germinando e proposta.

---

## V-07 — Registrar interesse em participar

**Como** aluno que quer entrar num projeto,

**quero** declarar interesse numa ideia,

**para** que quem a propôs saiba que pode me chamar.

### Pronto quando

- cada cartão tem um controle **"tenho interesse em participar"**;
- ao acionar, meu nome passa a constar na lista de interessados daquela ideia;
- a mesma pessoa não consegue se registrar duas vezes na mesma ideia;
- é possível desfazer o interesse, e o nome sai da lista;
- o número de interessados exibido no cartão corresponde ao tamanho da lista;
- o autor da ideia consegue visualizar a lista completa de interessados.

---

## V-08 — Não perder o que foi escrito

**Como** usuário,

**quero** não perder o que escrevi,

**para** não ter que digitar tudo de novo.

### Pronto quando

- os dados devem ser recuperados automaticamente ao recarregar a página;
- os dados são salvos automaticamente durante a edição.

---

## V-09 — Aviso de novo interessado

**Como** aluno com uma ideia publicada,

**quero** receber uma notificação no celular quando alguém demonstrar interesse,

**para** não perder a chance de formar grupo.

### Pronto quando

- ao registrar interesse, o autor recebe uma notificação no celular em até um minuto;
- a notificação mostra o nome de quem se interessou e o título da ideia;
- tocar na notificação abre a ideia correspondente.

---

# Caixa de entrada

Anotações de conversa. Ninguém escreveu direito ainda.

---

## V-10 — Ideias paradas

**Como** professor responsável por acompanhar os projetos,

**quero** identificar rapidamente as ideias que estão sem movimentação,

**para** incentivar que elas sejam retomadas ou encerradas.

### Pronto quando

- ideias sem atualizações por mais de 30 dias aparecem marcadas;
- existe um indicador visual mostrando que a ideia está parada;
- é possível listar apenas as ideias paradas;
- quando houver nova atividade, o indicador desaparece.

---

## V-11 — Relatório por curso

**Como** coordenador,

**quero** visualizar um relatório das ideias por curso,

**para** acompanhar a participação de cada área.

### Pronto quando

- o relatório mostra a quantidade de ideias por curso;
- mostra o número de alunos participantes;
- apresenta o total de projetos em cada estado;
- é possível selecionar um curso específico.

---

## V-12 — Exportar / importar o estado

**Como** administrador,

**quero** exportar e importar os dados do sistema,

**para** realizar backup ou restaurar informações.

### Pronto quando

- é possível exportar todos os dados em arquivo JSON;
- é possível importar um arquivo previamente exportado;
- os dados existentes são atualizados corretamente;
- caso o arquivo seja inválido, o sistema exibe uma mensagem de erro.

---

# Defeitos conhecidos

Nenhum destes foi priorizado. Estão aqui para não serem esquecidos.

- **B-01** — buscar `robotica` não encontra "Robótica"; buscar `Musica` não encontra "música".
- **B-02** — o número de apoios no cartão só muda depois que se refaz a busca.
- **B-03** — depois de clicar numa tag, não há como desfazer o filtro; só recarregando a página.
- **B-04** — quando a busca não encontra nada, o mural fica em branco, sem nenhuma explicação.
- **B-05** — título comprido vaza para fora do cartão e atravessa o cartão vizinho.
- **B-06** — a data aparece como `2026-03-14` em vez de `14/03/2026`.

<h1>Triagem</h1>
<i>A palavra dentro dos parênteses indica o estado da história antes da mesma ser corrigida pela nossa equipe</i>


V-02 (Errado) : A estrutura da história se alterou para a forma como, quero e para, além de inserirmos uma definição mais estruturada para quando estará pronto

V-03 (Incompleto): Adicionamos dois requisitos para quando o projeto estiver pronto:  não permitir títulos duplicados,  existir limite para o tamanho do resumo.

V-04 (Errado): Ajustamos para definir os conceitos de amigável e adicionamos mais um requisito para estar pronto os filtros podem ser utilizados junto com a pesquisa por palavras-chave.

V-05(Incompleto):  Adicionamos mais um requisito não funcional: o usuário recebe confirmação ao entrar ou sair do grupo.

V-06(Incompleto):  Adicionamos mais detalhes no para do cliente 

V-07(Incompleto): Adicionamos mais um requisito: o autor da ideia consegue visualizar a lista completa de interessados.

V-08 (Errado) : O pronto tem linguagem inadequada para um backlog, adicionamos então dois requisitos os dados devem ser recuperados automaticamente ao recarregar a página e os dados são salvos automaticamente durante a edição;


