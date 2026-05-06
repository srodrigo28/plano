# Projeto 2: Prompt Completo da Apresentação Comercial Interativa

## Objetivo do Projeto
Criar uma apresentação comercial em `HTML` com visual premium, leve e profissional para representar o modelo de coparticipação comercial da startup, com foco em clareza visual, confiança, tecnologia e capacidade de conversão para investidores e parceiros comerciais.

O projeto precisa comunicar:

- solidez do modelo de negócio;
- modernidade tecnológica;
- clareza sobre rentabilidade e retenções;
- profissionalismo comercial;
- facilidade de entendimento para o investidor.

## Entrega Principal
Desenvolver uma página `HTML` interativa, responsiva e visualmente sofisticada, com:

- apresentação institucional;
- explicação do modelo operacional;
- simulador financeiro;
- gráficos dinâmicos;
- tabela paginada customizada;
- persistência local de parâmetros;
- animações suaves de entrada e interação.

## Conteúdo Base do Projeto
O conteúdo textual, estratégico e financeiro parte do material consolidado em:

- `plano-5.md`;
- `plano-4.md`;
- documentos complementares da pasta do projeto.

## Tecnologias Utilizadas

### Estrutura Base
- `HTML5`
- `CSS3`
- `JavaScript ES Modules`

### Estilo e Interface
- `Tailwind CSS` via CDN
- `Bootstrap Icons`

### Gráficos e Visualização
- `Chart.js`

### Animações
- `Motion One`

### Máscaras e Tratamento de Entrada
- `IMask`

## Tecnologias Removidas Durante a Evolução
Inicialmente foi utilizada a biblioteca:

- `Simple-DataTables`

Porém ela foi removida porque apresentou limitações no comportamento visual e na paginação dinâmica quando a quantidade de ciclos mudava. No lugar dela foi criada uma solução própria em `JavaScript`, com controle total de:

- busca;
- paginação;
- quantidade de itens por página;
- renderização da tabela;
- atualização ao simular novos valores.

## Arquivo Principal da Interface
- `apresentacao-comercial.html`

## Direção Visual
O design deve seguir uma linha clara, elegante e comercial, evitando aparência pesada ou excessivamente técnica.

### Características visuais
- paleta em tons claros;
- sensação de leveza e sofisticação;
- blocos com transparência suave;
- sombras discretas;
- uso de gradientes leves no fundo;
- aparência institucional e tecnológica;
- legibilidade forte para métricas e números.

### Cores principais usadas
- areia clara;
- branco quente;
- azul suave;
- verde-azulado;
- dourado discreto;
- coral para contraste estratégico.

## Tipografia e Leitura
- títulos fortes e confiáveis;
- textos secundários suaves;
- números com destaque visual;
- estrutura de leitura rápida para apresentação comercial.

## Bibliotecas e Finalidades

### 1. Tailwind CSS
Usado para:

- layout responsivo;
- grids;
- espaçamento;
- cartões visuais;
- botões;
- seções institucionais;
- tipografia;
- controle rápido de estilo.

### 2. Bootstrap Icons
Usado para:

- ícones de tecnologia;
- crescimento;
- projeção;
- segurança;
- busca;
- paginação;
- simulação;
- gráficos e navegação visual.

### 3. Chart.js
Usado para:

- gráfico de crescimento do capital por ciclo;
- gráfico comparativo entre bruto, retenção e líquido;
- gráfico de distribuição da estrutura operacional.

### 4. Motion One
Usado para:

- animações de entrada;
- transições suaves entre seções;
- feedback visual no botão de simulação;
- reforço de sofisticação da interface.

### 5. IMask
Usado para:

- máscara monetária no padrão brasileiro;
- tratamento do campo de valor inicial;
- maior segurança na entrada de dados;
- leitura consistente de números em `Real Brasileiro`.

## Funcionalidades Implementadas

### 1. Hero Comercial
Bloco inicial com:

- mensagem principal;
- proposta de valor;
- botões de navegação;
- indicadores de crescimento bruto e líquido.

### 2. Seções Institucionais
Blocos explicando:

- campanhas conectadas;
- automação e dados;
- modelo orientado por métricas;
- liquidez com proteção;
- modelo operacional;
- distribuição financeira.

### 3. Simulador Financeiro
O simulador foi criado para permitir atualização dinâmica da projeção.

#### Campos do simulador
- `Valor inicial`
- `Qtd. de ciclos`
- `Lucro por ciclo (%)`
- `Retenção prevista (%)`

#### Regras aplicadas
- `Valor inicial` é editável com máscara brasileira;
- `Qtd. de ciclos` é editável;
- `Lucro por ciclo (%)` fica bloqueado como regra fixa do modelo;
- `Retenção prevista (%)` fica bloqueado como regra fixa do modelo.

### 4. Persistência de Dados
O simulador utiliza `localStorage` para salvar automaticamente:

- valor inicial;
- quantidade de ciclos;
- taxa de lucro por ciclo;
- retenção prevista.

Isso permite recarregar a página mantendo o último estado informado pelo usuário.

### 5. Cálculo Dinâmico
A simulação atualiza em tempo real:

- capital por ciclo;
- lucro projetado;
- saque parcial;
- reinvestimento;
- capital final;
- ganho bruto;
- retenção prevista;
- ganho líquido;
- percentual bruto;
- percentual líquido.

## Lógica de Negócio Aplicada na Simulação
Premissas atuais:

- `6%` de lucro por ciclo;
- `50%` do lucro como saque;
- `50%` do lucro como reinvestimento;
- `30%` de retenção prevista sobre o ganho bruto consolidado.

Essas regras alimentam:

- os cards principais;
- os textos explicativos;
- a tabela;
- os gráficos.

## Tabela Customizada
A tabela da projeção foi desenvolvida manualmente em `JavaScript`.

### Recursos implementados
- paginação própria;
- busca local;
- seletor de itens por página;
- atualização automática quando os ciclos mudam;
- feedback visual consistente;
- mensagens em português.

### Motivo da implementação manual
Garantir:

- controle visual total;
- maior estabilidade;
- adaptação ao número variável de ciclos;
- remoção de comportamentos inesperados de bibliotecas prontas.

## Gráficos Implementados

### 1. Evolução do Capital
Tipo:
- linha

Objetivo:
- mostrar o crescimento do capital a cada ciclo.

### 2. Bruto x Líquido
Tipo:
- barras

Objetivo:
- comparar ganho bruto anual, retenção prevista e ganho líquido.

### 3. Distribuição Operacional
Tipo:
- doughnut

Objetivo:
- representar visualmente a lógica de distribuição operacional.

## Requisitos de Experiência do Usuário
- interface leve;
- aparência premium;
- navegação simples;
- dados fáceis de entender;
- foco em credibilidade;
- boa leitura em desktop e mobile;
- interação suave sem exageros.

## Requisitos Técnicos
- uso de bibliotecas via CDN;
- funcionamento sem backend;
- código organizado em blocos semânticos;
- cálculos centralizados em JavaScript;
- máscara financeira local para o padrão brasileiro;
- persistência local com `localStorage`;
- gráficos atualizados com base nos dados simulados.

## Requisitos de Negócio Representados na Interface
- apresentação da startup como operação tecnológica e comercial;
- clareza entre projeção bruta e projeção líquida;
- reforço de retenções previstas;
- foco em transparência;
- proteção contra interpretação de promessa fixa de rendimento.

## Arquivos Relacionados
- `projeto-1.md`
- `apresentacao-comercial.html`
- `plano-4.md`
- `plano-5.md`

## Prompt Final Recomendado
Criar uma apresentação comercial interativa em `HTML`, com `Tailwind CSS`, `Bootstrap Icons`, `Chart.js`, `Motion One` e `IMask`, baseada no plano de coparticipação comercial da startup. A interface deve ter visual claro, sofisticado e comercial, com cards institucionais, gráficos dinâmicos, simulador financeiro com persistência local, campo monetário em padrão brasileiro, regras fixas de lucro e retenção, além de uma tabela própria paginada em JavaScript com busca e navegação visual. O objetivo é apresentar o modelo com credibilidade, clareza operacional e forte apelo comercial para investidores e parceiros.
