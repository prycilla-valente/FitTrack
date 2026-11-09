# FitTrack | Acompanhe seus treinos e hábitos

## Sobre o projeto

O **FitTrack** é um projeto desenvolvido como atividade prática do curso de Bootstrap, com o objetivo de aplicar os conceitos de construção de interfaces responsivas utilizando HTML5, CSS3 e Bootstrap 5.

A proposta é apresentar uma plataforma fictícia para acompanhamento de treinos, hábitos e evolução física, com diferentes componentes de interface, como navegação, cards, tabelas, formulários, modal e dashboard.

O projeto foi desenvolvido sem utilização do JavaScript do Bootstrap, conforme as orientações da atividade.

## Tecnologias utilizadas

- HTML5
- CSS3
- Bootstrap 5.0.2
- Bootstrap Icons 1.11.3
- Google Fonts — Lato

## Estrutura do projeto

    FitTrack/
    │
    ├── index.html
    │
    ├── css/
    │   └── styles.css
    │
    └── img/
        ├── favicon-16x16.png
        ├── fitness-svgrepo-com.svg
        └── foto-2.jpg

---

# Etapas desenvolvidas

## Etapa 1 — Navbar

Criação de uma barra de navegação responsiva, com identificação visual da plataforma e links para as principais seções.

Foram utilizadas classes do componente Navbar do Bootstrap, juntamente com utilitários de exibição para adaptar o menu a diferentes tamanhos de tela.

Como o JavaScript do Bootstrap não poderia ser utilizado, foi adotada uma alternativa em que o menu permanece visível e vertical em telas menores e horizontal em telas grandes.

## Etapa 2 — Hero Section

Desenvolvimento da seção inicial da página, contendo título, textos explicativos, botões de ação e imagem ilustrativa.

Foram utilizados o sistema de Grid do Bootstrap, classes de alinhamento e classes responsivas para alterar a ordem dos elementos conforme o tamanho da tela.

## Etapa 3 — Cards de conteúdo

Criação de 12 cards para apresentar os recursos da plataforma.

Os cards foram organizados com o sistema de colunas responsivas do Bootstrap:

- Uma coluna em dispositivos pequenos.
- Duas colunas em telas médias.
- Quatro colunas em telas grandes.

Também foram utilizadas classes de espaçamento, altura, bordas, sombras, flexbox e badges.

## Etapa 4 — Tabela profissional

Criação de uma tabela para apresentar o histórico de treinos, com informações sobre data, atividade, categoria, duração, calorias e status.

Foram aplicadas classes para adicionar bordas, listras alternadas, efeito hover, alinhamento vertical e rolagem horizontal em telas menores.

## Etapa 5 — Formulários

Desenvolvimento de dois formulários:

- **Cadastro:** campos para informações pessoais, e-mail, senha, telefone, seleção de opções, radio buttons e checkbox.
- **Contato:** campos para nome, e-mail, telefone, assunto e mensagem.

Foram utilizadas classes de formulários, organização em Grid, feedback visual de validação e agrupamento de campos.

## Etapa 6 — Modal sem JavaScript

Implementação de uma janela modal para simular a confirmação de registro de treino.

Como o JavaScript do Bootstrap não poderia ser utilizado, foi empregado o recurso de checkbox do HTML associado a seletores CSS para controlar a exibição da janela.

As classes utilitárias do Bootstrap foram utilizadas para posicionamento, alinhamento, cores e organização dos elementos.

## Etapa 7 — Responsividade

Aplicação de classes responsivas para controlar a exibição, o alinhamento e a organização dos elementos de acordo com a largura da tela.

Foram utilizados os breakpoints do Bootstrap para adaptar a experiência em dispositivos móveis, tablets e desktops.

## Etapa 8 — Sistema de design

Aplicação de diferentes cores, botões e badges disponibilizados pelo Bootstrap.

O objetivo foi explorar as opções visuais do framework e estabelecer uma identidade visual coerente com a proposta do FitTrack.

## Etapa 9 — Dashboard

Desenvolvimento de um painel administrativo com:

- Sidebar de navegação.
- Barra superior.
- Cards de métricas.
- Alertas informativos.
- Tabela de treinos recentes.

A estrutura do dashboard foi construída com CSS Grid e Flexbox, utilizando também classes utilitárias do Bootstrap.

A sidebar permanece na área lateral em telas grandes e fica inicialmente escondida em telas menores, podendo ser exibida por meio de um checkbox e CSS, sem JavaScript.

---

# Documentação das classes Bootstrap utilizadas

Esta seção apresenta as principais classes do Bootstrap utilizadas no projeto, organizadas por categoria, com a explicação de suas funcionalidades e exemplos de aplicação no FitTrack.

## 1. Sistema de Grid e colunas

O sistema de Grid permite organizar os elementos da página em linhas e colunas, facilitando a construção de layouts responsivos.

| Classe | Funcionalidade |
|---|---|
| `container` | Cria um contêiner centralizado, com largura máxima que varia conforme o breakpoint. |
| `row` | Cria uma linha que organiza as colunas do Grid. |
| `col` | Define uma coluna com distribuição automática do espaço disponível. |
| `col-12` | Faz o elemento ocupar as 12 colunas disponíveis. |
| `col-md-4` | Faz o elemento ocupar 4 das 12 colunas a partir do breakpoint md. |
| `col-md-6` | Faz o elemento ocupar metade da linha a partir do breakpoint md. |
| `col-md-8` | Faz o elemento ocupar 8 das 12 colunas a partir do breakpoint md. |
| `row-cols-1` | Define uma coluna por linha. |
| `row-cols-md-2` | Define duas colunas por linha a partir do breakpoint md. |
| `row-cols-lg-4` | Define quatro colunas por linha a partir do breakpoint lg. |
| `g-3` | Define espaçamento entre as colunas e linhas do Grid. |
| `g-4` | Define um espaçamento maior entre as colunas e linhas do Grid. |

**Exemplo no projeto:**

    <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4 g-4">

Essa combinação permite que os cards sejam exibidos em uma coluna nos dispositivos menores, duas colunas em telas médias e quatro colunas em telas grandes.

## 2. Responsividade e exibição

As classes responsivas controlam quando um elemento deve aparecer ou desaparecer conforme o tamanho da tela.

| Classe | Funcionalidade |
|---|---|
| `d-none` | Oculta o elemento. |
| `d-block` | Exibe o elemento como bloco. |
| `d-flex` | Define o elemento como um contêiner Flexbox. |
| `d-grid` | Define o elemento como um contêiner Grid. |
| `d-inline` | Exibe o elemento em linha. |
| `d-inline-block` | Exibe o elemento como bloco em linha. |
| `d-lg-block` | Exibe o elemento como bloco a partir do breakpoint lg. |
| `d-lg-flex` | Exibe o elemento como Flexbox a partir do breakpoint lg. |
| `d-md-block` | Exibe o elemento como bloco a partir do breakpoint md. |
| `d-md-inline` | Exibe o elemento em linha a partir do breakpoint md. |
| `d-md-table-cell` | Exibe o elemento como célula de tabela a partir do breakpoint md. |
| `d-sm-inline` | Exibe o elemento em linha a partir do breakpoint sm. |
| `d-sm-inline-block` | Exibe o elemento como bloco em linha a partir do breakpoint sm. |

**Exemplo no projeto:**

    <p class="d-none d-md-block">
        Registre treinos, metas, alimentação, sono e hidratação.
    </p>

Nesse exemplo, o texto fica oculto em telas menores e aparece a partir do breakpoint md.

## 3. Flexbox e alinhamento

As classes de Flexbox permitem organizar os elementos, controlar seu alinhamento e distribuir o espaço entre eles.

| Classe | Funcionalidade |
|---|---|
| `flex-column` | Organiza os elementos verticalmente. |
| `justify-content-center` | Centraliza os elementos no eixo principal. |
| `justify-content-between` | Distribui os elementos com espaço entre eles. |
| `justify-content-end` | Alinha os elementos ao final do eixo principal. |
| `justify-content-sm-center` | Centraliza os elementos a partir do breakpoint sm. |
| `justify-content-md-start` | Alinha os elementos ao início a partir do breakpoint md. |
| `align-items-center` | Centraliza os elementos no eixo transversal. |
| `align-self-start` | Alinha individualmente um elemento ao início do eixo transversal. |
| `align-middle` | Alinha verticalmente o conteúdo de células de tabela. |
| `gap-2` | Define espaçamento entre os elementos de um contêiner flex ou grid. |
| `gap-3` | Define um espaçamento maior entre os elementos. |

**Exemplo no projeto:**

    <div class="card-body d-flex flex-column">

O conteúdo do card é organizado verticalmente por meio do Flexbox.

A classe `mt-auto`, explicada na seção de espaçamento, também é utilizada para manter os botões alinhados na parte inferior dos cards.

## 4. Espaçamento: margem e padding

O Bootstrap disponibiliza classes para controlar os espaços internos e externos dos elementos.

As letras utilizadas nas classes representam:

- `m`: margin (margem).
- `p`: padding (espaçamento interno).
- `t`: top (superior).
- `b`: bottom (inferior).
- `s`: start (início).
- `e`: end (final).
- `x`: horizontal.
- `y`: vertical.

| Classe | Funcionalidade |
|---|---|
| `m-0` | Remove a margem. |
| `mb-0` | Remove a margem inferior. |
| `mb-1` | Adiciona uma pequena margem inferior. |
| `mb-2` | Adiciona margem inferior. |
| `mb-3` | Adiciona margem inferior maior. |
| `mb-4` | Adiciona margem inferior ainda maior. |
| `mb-5` | Adiciona uma margem inferior ampla. |
| `me-1` | Adiciona margem no final do elemento. |
| `me-auto` | Utiliza margem automática no final do elemento. |
| `mt-auto` | Utiliza margem automática no topo, ocupando o espaço disponível. |
| `mt-3` | Adiciona margem superior. |
| `p-3` | Adiciona espaçamento interno em todos os lados. |
| `p-md-4` | Adiciona padding 4 a partir do breakpoint md. |
| `px-3` | Adiciona padding horizontal. |
| `px-md-4` | Adiciona padding horizontal a partir do breakpoint md. |
| `py-3` | Adiciona padding vertical. |
| `py-5` | Adiciona padding vertical maior. |

**Exemplo no projeto:**

    <section class="py-5">

A classe adiciona espaçamento interno na parte superior e inferior da seção.

## 5. Tipografia e textos

As classes de tipografia permitem controlar o tamanho, o peso e a aparência dos textos.

| Classe | Funcionalidade |
|---|---|
| `display-5` | Aplica um estilo de título de destaque, com tamanho maior. |
| `lead` | Destaca um parágrafo com aparência de texto introdutório. |
| `small` | Aplica tamanho de fonte menor. |
| `h3` | Aplica a aparência visual de um título h3. |
| `h4` | Aplica a aparência visual de um título h4. |
| `h5` | Aplica a aparência visual de um título h5. |
| `fw-bold` | Aplica peso de fonte em negrito. |
| `fw-normal` | Aplica peso de fonte normal. |
| `text-center` | Centraliza o texto. |
| `text-start` | Alinha o texto ao início. |
| `text-md-start` | Alinha o texto ao início a partir do breakpoint md. |
| `text-success` | Aplica a cor de texto associada ao sucesso. |
| `text-warning` | Aplica a cor de texto associada à atenção. |
| `text-white` | Aplica a cor branca ao texto. |

## 6. Cores e fundos

As classes de cores ajudam a estabelecer uma identidade visual e a transmitir informações por meio de diferentes estados.

| Classe | Funcionalidade |
|---|---|
| `bg-primary` | Aplica a cor de fundo principal do Bootstrap. |
| `bg-secondary` | Aplica a cor de fundo secundária. |
| `bg-success` | Aplica a cor associada ao sucesso. |
| `bg-warning` | Aplica a cor associada à atenção. |
| `bg-info` | Aplica a cor associada a informações. |
| `bg-danger` | Aplica a cor associada a erros ou situações de perigo. |
| `bg-light` | Aplica um fundo claro. |
| `bg-dark` | Aplica um fundo escuro. |
| `bg-white` | Aplica fundo branco. |
| `bg-success-subtle` | Aplica uma tonalidade suave da cor de sucesso. |
| `bg-warning-subtle` | Aplica uma tonalidade suave da cor de atenção. |

No projeto, também foram criadas classes personalizadas, como `bg-primary-color`, `bg-secondary-color`, `primary-color` e `secondary-color`, para aplicar a identidade visual própria do FitTrack.

## 7. Botões e badges

### Botões

| Classe | Funcionalidade |
|---|---|
| `btn` | Classe base necessária para criar um botão Bootstrap. |
| `btn-primary` | Botão com aparência principal. |
| `btn-outline-secondary` | Botão secundário com contorno. |
| `btn-success` | Botão associado a uma ação de sucesso. |
| `btn-danger` | Botão associado a uma ação de perigo ou cancelamento. |
| `btn-lg` | Aumenta o tamanho do botão. |
| `btn-close` | Cria um botão visual de fechamento. |

### Badges

| Classe | Funcionalidade |
|---|---|
| `badge` | Define o elemento como um rótulo visual. |
| `bg-warning` | Aplica fundo de atenção ao badge. |
| `bg-success` | Aplica fundo de sucesso ao badge. |
| `bg-info` | Aplica fundo informativo ao badge. |
| `bg-danger` | Aplica fundo de perigo ao badge. |
| `bg-secondary` | Aplica fundo secundário ao badge. |

Os badges foram utilizados para destacar informações como novidades, recursos essenciais, status de treinos e atividades em andamento.

## 8. Cards, bordas e sombras

| Classe | Funcionalidade |
|---|---|
| `card` | Cria um componente de cartão. |
| `card-body` | Define a área principal de conteúdo do card. |
| `card-title` | Aplica estilo ao título do card. |
| `card-text` | Aplica estilo ao texto do card. |
| `card-header` | Define o cabeçalho do card. |
| `card-footer` | Define o rodapé do card. |
| `border-0` | Remove as bordas. |
| `border-bottom` | Adiciona borda inferior. |
| `rounded` | Arredonda os cantos do elemento. |
| `rounded-3` | Aplica arredondamento de cantos com intensidade 3. |
| `shadow` | Adiciona sombra ao elemento. |
| `shadow-sm` | Adiciona sombra pequena. |
| `shadow-lg` | Adiciona sombra maior. |

## 9. Tabelas

| Classe | Funcionalidade |
|---|---|
| `table` | Aplica a estrutura visual básica de uma tabela Bootstrap. |
| `table-responsive` | Permite rolagem horizontal da tabela quando necessário. |
| `table-bordered` | Adiciona bordas às células. |
| `table-striped` | Aplica listras alternadas às linhas. |
| `table-hover` | Adiciona efeito visual ao passar o mouse sobre as linhas. |
| `table-dark` | Aplica aparência escura à tabela ou ao cabeçalho. |
| `align-middle` | Centraliza verticalmente o conteúdo das células. |
| `mb-0` | Remove a margem inferior da tabela. |

## 10. Formulários

| Classe | Funcionalidade |
|---|---|
| `form-label` | Padroniza a aparência dos rótulos dos campos. |
| `form-control` | Aplica estilo aos campos de entrada de texto. |
| `form-select` | Aplica estilo aos campos de seleção. |
| `form-check` | Agrupa elementos de checkbox ou radio. |
| `form-check-input` | Aplica estilo ao campo checkbox ou radio. |
| `form-check-label` | Aplica estilo ao texto associado ao checkbox ou radio. |
| `form-text` | Aplica estilo a um texto auxiliar do formulário. |
| `input-group` | Agrupa campos e elementos adicionais em uma única estrutura visual. |
| `input-group-text` | Estiliza um texto ou elemento complementar dentro do input group. |
| `is-valid` | Indica visualmente um campo válido. |
| `is-invalid` | Indica visualmente um campo inválido. |
| `valid-feedback` | Exibe uma mensagem de retorno positivo. |
| `invalid-feedback` | Exibe uma mensagem de retorno negativo. |

## 11. Alertas

| Classe | Funcionalidade |
|---|---|
| `alert` | Classe base para criação de alertas. |
| `alert-success` | Alerta de sucesso. |
| `alert-warning` | Alerta de atenção. |
| `alert-danger` | Alerta de erro ou perigo. |

No dashboard, os alertas são utilizados para apresentar informações sobre treinos concluídos, atividades em andamento e atividades canceladas.

## 12. Imagens

| Classe | Funcionalidade |
|---|---|
| `img-fluid` | Faz a imagem se adaptar à largura do elemento pai, mantendo sua proporção. |

Foi utilizada na imagem principal da Hero Section para garantir que ela se adapte ao espaço disponível em diferentes dispositivos.

## 13. Modal e posicionamento

| Classe | Funcionalidade |
|---|---|
| `position-fixed` | Posiciona o elemento em relação à janela de visualização. |
| `position-absolute` | Posiciona o elemento em relação ao ancestral posicionado mais próximo. |
| `position-relative` | Cria um contexto de posicionamento para elementos filhos. |
| `top-0` | Posiciona o elemento no topo. |
| `start-0` | Posiciona o elemento no início horizontal. |
| `w-100` | Define largura de 100%. |
| `h-100` | Define altura de 100%. |

Essas classes foram utilizadas na construção visual do modal, em conjunto com regras personalizadas de CSS para controlar sua exibição sem JavaScript.

## 14. Navbar e navegação

| Classe | Funcionalidade |
|---|---|
| `navbar` | Define a estrutura principal da barra de navegação. |
| `navbar-expand-lg` | Expande a navegação horizontalmente a partir do breakpoint lg. |
| `navbar-brand` | Estiliza a identificação ou marca da navegação. |
| `navbar-nav` | Define a lista de links da navegação. |
| `navbar-collapse` | Define a área de conteúdo recolhível da navbar. |
| `nav-item` | Define um item da navegação. |
| `nav-link` | Estiliza um link da navegação. |
| `active` | Indica visualmente o item ativo. |
| `sticky-top` | Mantém o elemento aderido ao topo durante a rolagem. |

---

# Bootstrap Icons

Além das classes do Bootstrap, o projeto utiliza o pacote Bootstrap Icons para inserir ícones em diferentes partes da interface.

Os ícones são adicionados por meio da classe base `bi` e de uma classe específica para cada ícone.

Exemplos utilizados:

| Classe | Representação |
|---|---|
| `bi bi-activity` | Atividade física |
| `bi bi-person-plus` | Cadastro de usuário |
| `bi bi-calendar-event` | Calendário |
| `bi bi-clock` | Tempo ou duração |
| `bi bi-fire` | Calorias |
| `bi bi-check-circle-fill` | Confirmação |
| `bi bi-trophy` | Conquistas |
| `bi bi-water` | Hidratação |
| `bi bi-list` | Menu |
| `bi bi-gear` | Configurações |
| `bi bi-person-circle` | Perfil do usuário |

Também foram utilizadas classes de espaçamento, como `me-1` e `me-2`, para controlar a distância entre os ícones e os textos.

---

# CSS personalizado

Embora o Bootstrap ofereça diversos recursos prontos, foi necessário utilizar CSS próprio para atender às características visuais e funcionais do projeto.

As principais personalizações foram:

- **Identidade visual:** criação de classes próprias para cores, fontes e fundos.
- **Navbar:** ajustes de cores, logotipo e efeitos de interação.
- **Hero:** definição de altura mínima e ajustes específicos da imagem.
- **Cards:** aplicação de efeitos visuais ao passar o mouse.
- **Tabelas:** ajustes de espaçamento e comportamento do conteúdo.
- **Botões:** criação de estilos personalizados para combinar com a identidade visual.
- **Modal:** controle de exibição utilizando checkbox e seletores CSS, sem JavaScript.
- **Dashboard:** construção da estrutura principal com CSS Grid e organização interna com Flexbox.
- **Sidebar:** controle de exibição em dispositivos menores utilizando checkbox e CSS.
- **Responsividade:** ajustes específicos por meio de media queries.

O CSS personalizado complementa o Bootstrap quando os recursos nativos do framework não atendem exatamente ao comportamento ou à aparência desejada.

---

# Principais desafios

Durante o desenvolvimento do projeto, alguns pontos exigiram maior atenção e pesquisa:

- Compreender o funcionamento do sistema de Grid e dos breakpoints responsivos.
- Escolher corretamente as classes de espaçamento e alinhamento.
- Organizar os cards para manter alturas e botões alinhados.
- Adaptar tabelas para telas menores sem comprometer a leitura.
- Construir formulários com diferentes tipos de campos e estados visuais.
- Implementar o modal sem utilizar JavaScript.
- Desenvolver o dashboard utilizando CSS Grid e Flexbox.
- Criar uma sidebar responsiva sem recorrer a `position: absolute`.

Esses desafios contribuíram para ampliar o entendimento sobre o Bootstrap e sobre a integração entre HTML e CSS.

# Considerações finais

O desenvolvimento do FitTrack permitiu aplicar, na prática, diversos recursos do Bootstrap 5, especialmente o sistema de Grid, as classes utilitárias, os componentes visuais e as ferramentas de responsividade.

Além de utilizar classes prontas, o projeto também exigiu a compreensão de como combiná-las e quando recorrer ao CSS personalizado para alcançar o resultado esperado.

A documentação das classes utilizadas foi incluída como material de consulta, com o objetivo de registrar o aprendizado e facilitar a reutilização desses recursos em projetos futuros.




