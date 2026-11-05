# HemoAtlas

**Encontre onde doar. Entenda onde faz falta.**

Plataforma web para encontrar locais de doação de sangue, consultar horários de atendimento e acompanhar os estoques dos hemocentros.

**FMU Tech Inovação · 2026.2 · Ciência da Computação · 2º semestre · ODS 3**

## Sumário

- [Sobre o projeto](#sobre-o-projeto)
- [Problema](#problema)
- [Público-alvo](#publico)
- [Solução](#solucao)
- [Funcionalidades](#funcionalidades)
- [Fontes de dados](#fontes)
- [Tecnologias e ferramentas](#tecnologias)
- [Identidade visual](#identidade)
- [Equipe](#equipe)
- [Pitch](#pitch)

<a id="sobre-o-projeto"></a>
## Sobre o projeto

O **HemoAtlas** reúne informações sobre redes e unidades de coleta de sangue em um mapa interativo do Brasil. A proposta é facilitar a busca por locais de doação e dar visibilidade às necessidades divulgadas pelas instituições.

O projeto está alinhado à **ODS 3 — Saúde e Bem-Estar**, ao facilitar o acesso à informação e incentivar a doação de sangue.

<a id="problema"></a>
## Problema

Endereços, horários e informações sobre estoques de sangue estão distribuídos em diferentes sites. Isso dificulta encontrar um local para doar e saber quais instituições precisam de determinado tipo sanguíneo.

O HemoAtlas busca reunir essas informações em um só lugar, com fontes identificadas e indicação de atualização.

<a id="publico"></a>
## Público-alvo

- Pessoas que desejam doar sangue pela primeira vez.
- Doadores que querem acompanhar suas doações e planejar o retorno.
- Pessoas que procuram unidades de coleta em sua cidade ou estado.

<a id="solucao"></a>
## Solução

Um mapa do Brasil em perspectiva permite selecionar um estado e visualizar suas unidades de coleta. Ao clicar em um marcador, o usuário encontra endereço, horários, contato e necessidades de sangue, quando divulgadas pela instituição.

Os locais também podem ser consultados em uma lista, com filtros por estado, cidade, rede e tipo sanguíneo. A área do doador reúne preferências, histórico de doações e lembretes de retorno.

<a id="funcionalidades"></a>
## Funcionalidades

| Funcionalidade | Descrição |
|---|---|
| Mapa interativo | Visualização do Brasil em perspectiva, com divisões estaduais |
| Navegação por estado | Aproximação animada para o estado selecionado e opção de voltar ao Brasil |
| Redes e unidades | Organização dos locais de coleta por rede e unidade |
| Busca e filtros | Consulta por estado, cidade, rede e tipo sanguíneo |
| Informações da unidade | Endereço, horários de coleta, contato e fonte oficial |
| Situação dos estoques | Consulta às necessidades por tipo sanguíneo divulgadas pelas instituições |
| Painel geral | Resumo das necessidades das redes e unidades acompanhadas |
| Perfil do doador | Registro de preferências e tipo sanguíneo |
| Histórico de doações | Registro e consulta das doações |
| Lembretes | Avisos de retorno |

<a id="fontes"></a>
## Fontes de dados

As informações serão obtidas em bases públicas e nos sites oficiais das instituições.

| Fonte | Informações utilizadas |
|---|---|
| [CNES / DATASUS](https://wiki.datasus.gov.br/cnes/index.php/Portal_CNES) | Identificação e dados cadastrais dos estabelecimentos |
| [Ministério da Saúde](https://www.gov.br/saude/pt-br/composicao/saes/doacao-de-sangue/arquivos/lista-de-hemocentros.pdf/view) | Relação de hemocentros para complementar o levantamento |
| [IBGE](https://servicodados.ibge.gov.br/api/docs/malhas?versao=3) | Contornos do Brasil e dos estados para o mapa |
| [Hemominas](https://hemominas.mg.gov.br/) | Informações institucionais e situação dos estoques divulgados |
| [HEMOSC](https://www.hemosc.org.br/index.php) | Informações sobre a rede e seus estoques |
| [Fundação Pró-Sangue](https://prosangue.sp.gov.br/reqestoque/posicao_estoque.php) | Situação de estoque divulgada pela instituição |
| [Hemoba](https://www.ba.gov.br/hemoba/onde-doar) | Unidades, endereços, contatos e horários de coleta |

O catálogo será ampliado com outras fontes oficiais. Cada informação de estoque terá sua fonte e a data disponível de atualização. Indicadores de uma rede serão identificados como dados da rede, sem atribuí-los individualmente a cada unidade. Quando não houver divulgação, o site mostrará **“estoque não informado”**.

<a id="tecnologias"></a>
## Tecnologias e ferramentas

### Tecnologias

| Tecnologia | Uso |
|---|---|
| HTML | Estrutura da página |
| JavaScript | Filtros, navegação e tratamento dos dados |
| React | Organização dos componentes e atualização da interface |
| CSS | Estilos, identidade visual e adaptação a diferentes telas |
| MapLibre GL JS | Mapa em perspectiva, marcadores e animações |
| GeoJSON | Representação dos estados e pontos no mapa |
| JSON | Organização dos dados das redes, unidades e estoques |

A aplicação será executada localmente, sem back-end ou banco de dados compartilhado. O React será utilizado sem JSX. Os dados do doador permanecerão no navegador, sem autenticação de conta, e os lembretes serão exibidos dentro do site.

### Ferramentas

| Ferramenta | Finalidade |
|---|---|
| VS Code | Desenvolvimento do código |
| Git e GitHub | Versionamento e organização do projeto |
| Figma | Planejamento das telas e da identidade visual |

<a id="identidade"></a>
## Identidade visual

Logo e Identidade visual localizados em:
- [Identidade Visual](./Identidade%20Visual/)
- [Logos](./Logos/)

### Conceito

O nome **HemoAtlas** une a referência ao sangue à ideia de um atlas: um mapa que ajuda a localizar unidades e consultar suas necessidades.

### Paleta de cores

#### Principais

| Cor | HEX | Aplicação |
|---|---|---|
| Vermelho Hemo | `#B91C3C` | Marca e botões principais |
| Azul-petróleo | `#12343B` | Títulos e navegação |

#### Secundárias

| Cor | HEX | Aplicação |
|---|---|---|
| Verde-petróleo | `#0F766E` | Seleção no mapa e elementos de apoio |
| Rosa suave | `#FFF1F2` | Fundos de destaque |
| Verde suave | `#E6F4F1` | Fundos de informações complementares |

#### Indicadores

| Cor | HEX | Aplicação |
|---|---|---|
| Vermelho | `#B91C1C` | Necessidade crítica |
| Âmbar | `#92400E` | Atenção ou estoque baixo |
| Verde | `#166534` | Estoque adequado |
| Cinza | `#64748B` | Informação indisponível |

Os indicadores terão rótulos para que a informação não dependa apenas da cor.

#### Neutros

| Cor | HEX | Aplicação |
|---|---|---|
| Branco | `#FFFFFF` | Cartões e fundos |
| Gelo | `#F8FAFC` | Fundo geral |
| Cinza claro | `#E2E8F0` | Divisórias e contornos |
| Grafite | `#1E293B` | Texto principal |

### Tipografia

| Fonte | Pesos | Uso |
|---|---|---|
| [Manrope](https://fonts.google.com/specimen/Manrope) | 600 e 700 | Títulos e marca |
| [Inter](https://fonts.google.com/specimen/Inter) | 400, 500 e 600 | Textos, filtros e botões |

<a id="equipe"></a>
## Equipe

| Integrante | RA | Curso e semestre |
|---|---|---|
| Brenno Oliveira Souza | 2026108788 | Ciência da Computação — 2º semestre |
| Murillo Manoel Silva Mendes | 2026104915 | Ciência da Computação — 2º semestre |
| Rayssa Morais de Aquino | 2026112326 | Ciência da Computação — 2º semestre |
| Ahmad Fayaz Kohistani | 2026114693 | Ciência da Computação — 2º semestre |

<a id="pitch"></a>
## Pitch

O HemoAtlas conecta a vontade de doar à informação sobre onde ajudar. Em um mapa interativo do Brasil, reúne unidades de coleta, horários e necessidades de sangue divulgadas por fontes oficiais. Com filtros por localização e tipo sanguíneo, histórico de doações e lembretes de retorno, o projeto busca facilitar a escolha de onde doar e incentivar a continuidade das doações. Seu diferencial é apresentar as informações por rede e unidade, com estoques atualizados.
