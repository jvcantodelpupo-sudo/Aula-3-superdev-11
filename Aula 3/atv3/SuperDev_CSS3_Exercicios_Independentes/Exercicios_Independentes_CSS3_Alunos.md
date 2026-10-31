# SuperDev — CSS3 | Exercícios independentes

## Regras gerais

O professor está usando uma página de cafeteria para **demonstrar** os conceitos. Nos exercícios abaixo você trabalhará em **outras páginas, com outros problemas**. Não copie o CSS da cafeteria: escolha como resolver cada desafio.

- Você recebe arquivos HTML prontos, com a estrutura e as classes necessárias.
- Edite somente o `estilos.css` de cada exercício, exceto quando uma tarefa pedir explicitamente uma alteração no HTML.
- Use apenas CSS, sem frameworks e sem JavaScript.
- Teste no navegador e use o DevTools para investigar.
- Não é necessário copiar um layout exato. Os objetivos visuais e os comportamentos descritos abaixo são os critérios de conclusão.

> **Organização:** as atividades estão em ordem de conteúdo, não precisam ser todas feitas de uma vez. O professor libera cada uma após a explicação correspondente.

---

## Exercício 1 — Central de avisos da Base Orion
**Quando usar:** após seletores, cores e tipografia.  
**Tempo sugerido:** 20–25 minutos.  
**Arquivos:** `01-central-alertas/index.html` e `estilos.css`.

### Situação
A página já mostra os comunicados de uma estação espacial, mas todos parecem iguais. Você precisa criar uma **hierarquia visual** para ajudar a equipe a identificar rapidamente os avisos importantes.

### Entregáveis

1. Crie uma aparência própria para o cabeçalho, diferente do corpo da página.
2. Faça o título principal se destacar dos demais títulos e escolha uma fonte legível.
3. Dê uma aparência comum a **todos** os comunicados.
4. O comunicado **urgente** precisa se destacar visualmente dos outros, sem alterar o HTML.
5. O comunicado **concluído** deve ser visualmente diferente do urgente e do informativo.
6. Os links do menu devem ser distinguíveis dos demais links da página.
7. Teste se os textos continuam legíveis quando você escolhe uma cor de fundo mais escura.

**Para refletir:** quais alterações você resolveu com seletor de elemento? Quais exigiram classe? Por quê?

**Extra (somente depois de estudar pseudo-classes):** mostre um efeito ao passar o mouse nos links e um indicador visível ao navegar usando Tab.

---

## Exercício 2 — Ingresso do Cinema Órbita
**Quando usar:** após Box Model e `box-sizing`.  
**Tempo sugerido:** 25–30 minutos.  
**Arquivos:** `02-ingresso-cinema/index.html` e `estilos.css`.

### Situação
O cinema precisa que seu ingresso digital pareça um **ingresso físico destacável**, e não um texto solto na página. Você será responsável pela disposição dos espaços.

### Entregáveis

1. O ingresso deve ter uma cor de fundo diferente do fundo da página.
2. Deve existir uma borda visível ao redor do ingresso.
3. O conteúdo **não pode ficar grudado** na borda.
4. O ingresso deve ficar separado do cabeçalho e da mensagem que vem depois dele.
5. Escolha uma largura para o ingresso e centralize-o horizontalmente.
6. A área `.detalhes` deve parecer um bloco interno separado do título do filme.
7. Use o DevTools para identificar e mostrar as áreas de **content, padding, border e margin**.

### Experimento obrigatório

- Defina uma largura de **360px** para `.ingresso`.
- Defina `padding: 24px` e uma borda de `6px`.
- Observe a largura externa no DevTools usando `content-box`.
- Troque apenas `box-sizing` para `border-box` e compare.
- **Anote:** por que a largura externa muda mesmo mantendo `width: 360px`?

**Desafio extra:** construa uma segunda versão do ingresso com espaço interno diferente, mas mesma largura externa.

---

## Exercício 3 — Agenda Cultural Cidade Viva
**Quando usar:** após unidades, dimensões e `display`.  
**Tempo sugerido:** 20–25 minutos.  
**Arquivos:** `03-agenda-cultural/index.html` e `estilos.css`.

### Situação
A agenda tem categorias de eventos e links de ação. Você precisa organizar a leitura sem usar Flexbox ou Grid (ainda).

### Entregáveis

1. O conteúdo principal deve ter uma largura confortável para leitura e não ocupar toda a tela em monitores grandes.
2. Centralize esse conteúdo horizontalmente.
3. Cada seção de evento deve ter seu próprio espaçamento, borda ou fundo.
4. Transforme os links **Saiba mais** em elementos com aparência de botão, mantendo o funcionamento dos links.
5. Os links de categoria devem aparecer próximos, com espaçamento que permita clicar sem dificuldade.
6. Use pelo menos uma unidade relativa em um tamanho de texto e outra em um espaçamento.
7. Redimensione o navegador e observe se o conteúdo continua utilizável.

### Experimento obrigatório

Altere o `display` de um dos links `.acao` entre `inline`, `block` e `inline-block`.

Responda: **em qual deles a largura do link e o padding vertical são mais fáceis de controlar sem ocupar a linha toda?**

**Extra:** estilize `:hover` e `:focus-visible` para os links de ação.

---

## Exercício 4 — Detetive de CSS: Missão Depuração
**Quando usar:** depois que os alunos já conhecem seletores, especificidade, Box Model e `display`.  
**Tempo sugerido:** 15–20 minutos.  
**Arquivos:** `04-debugging/index.html` e `estilos.css`.

### Situação
Outro desenvolvedor escreveu o CSS e a página está visualmente inconsistente. Sua tarefa é **descobrir as causas**, não apenas trocar valores aleatoriamente.

Encontre e corrija os quatro problemas indicados nos comentários do CSS:

1. A cor de fundo do aviso importante não está sendo aplicada como esperado.
2. O link com aparência de botão tem um comportamento de espaçamento estranho.
3. A caixa está mais larga do que o valor declarado em `width`.
4. Uma regra não está selecionando o título do aviso.

**Regra:** é proibido resolver usando `!important`.

**Entregável:** para cada erro, escreva um comentário com a causa do problema e a correção utilizada.

---

## Projeto opcional — Escolha um dos três e faça uma versão própria
**Quando usar:** apenas se sobrar tempo (30–40 minutos).

Escolha **uma** das páginas anteriores e reconstrua sua identidade visual com outras cores, fontes, bordas, espaçamentos e estados de interação. Não reutilize o CSS da demonstração do professor.

### Checklist de autonomia

- [ ] Consigo explicar por que escolhi cada seletor.
- [ ] Sei diferenciar espaço dentro e fora da borda.
- [ ] Consigo usar o DevTools para investigar uma regra.
- [ ] Sei identificar quando uma regra de CSS foi sobrescrita.
- [ ] Meu CSS está em arquivo externo.
- [ ] Testei a página com janela mais estreita.

> **Dica de investigação:** se algo não funcionar, antes de pedir a resposta, verifique se o seletor realmente encontra o elemento e se outra regra não está prevalecendo.
