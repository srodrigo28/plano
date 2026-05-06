# Plano de Revisao da Apresentacao

Data de referencia desta revisao: 6 de maio de 2026.

Este documento nao substitui parecer juridico. Ele organiza os principais ajustes de linguagem, estrutura e posicionamento para reduzir risco regulatorio percebido e aumentar a confianca do investidor.

## Objetivo

Melhorar o `index.html` para:

- reduzir termos que podem soar como oferta publica irregular ou promessa de rentabilidade
- aumentar coerencia entre proposta comercial, narrativa financeira e forma juridica
- transmitir mais seriedade, governanca e previsibilidade ao investidor
- preparar a apresentacao para revisao posterior por advogado societario e regulatorio

## Base regulatoria usada nesta revisao

Fontes oficiais consultadas em 6 de maio de 2026:

- Lei 6.385/1976, art. 2o, IX: quando ofertados publicamente, contratos que gerem direito de participacao, parceria ou remuneracao e cujos rendimentos venham do esforco do empreendedor podem ser tratados como valores mobiliarios.
  - https://www.planalto.gov.br/ccivil_03/leis/l6385.htm
- Portal do Investidor: definicao ampla de valores mobiliarios e contratos de investimento coletivo.
  - https://www.gov.br/investidor/pt-br/investir/como-investir/conheca-o-mercado-de-capitais/o-que-sao-valores-mobiliarios
- Portal do Investidor: crowdfunding de investimento e regulacao da CVM.
  - https://www.gov.br/investidor/pt-br/investir/tipos-de-investimentos/crowdfunding-de-investimento/o-crowdfunding-de-investimento-e-a-regulacao-da-cvm
- Portal do Investidor: oferta irregular de contratos de investimento coletivo.
  - https://www.gov.br/investidor/pt-br/investir/cuidados-ao-investir/evitando-problemas/principais-fraudes-e-esquemas-irregulares/oferta-irregular-de-contratos-de-investimento-coletivo
- CVM: ofertas publicas.
  - https://www.gov.br/cvm/pt-br/assuntos/regulados/consultas-por-participante/ofertas-publicas/saiba-mais-sobre-ofertas-publicas
- CVM: ofertas e atuacoes irregulares.
  - https://www.gov.br/cvm/pt-br/assuntos/protecao/alertas/ofertas-atuacoes-irregulares

Inferencia usada nesta revisao:

- Como a pagina divulga captação com expectativa de remuneracao, participacao ou retorno, e usa linguagem ampla de apresentacao comercial a investidores, ha risco de a comunicacao ser lida como oferta publica ou convite amplo de investimento se circular sem controle.

## Resumo executivo

Hoje a apresentacao esta comercialmente forte, mas ainda mistura:

- linguagem de sociedade
- linguagem de renda/retorno
- linguagem de garantia
- linguagem de promessa mensal

Esse conjunto pode gerar dois problemas ao mesmo tempo:

- risco regulatorio: parecer uma oferta publica de valor mobiliario ou contrato de investimento coletivo
- risco comercial: investidor sofisticado pode desconfiar de promessa excessivamente redonda, sobretudo em `R$ 3.400,00 por mes`, `4x`, `garantia`, `desde o mes 1`

## Prioridade alta

### 1. Reduzir linguagem de promessa de retorno fixo

Trechos sensiveis:

- [index.html](c:\plano\e-vendas\modelo\index.html:252)
- [index.html](c:\plano\e-vendas\modelo\index.html:367)
- [index.html](c:\plano\e-vendas\modelo\index.html:430)
- [index.html](c:\plano\e-vendas\modelo\index.html:471)
- [index.html](c:\plano\e-vendas\modelo\index.html:510)
- [index.html](c:\plano\e-vendas\modelo\index.html:517)
- [index.html](c:\plano\e-vendas\modelo\index.html:524)
- [index.html](c:\plano\e-vendas\modelo\index.html:543)
- [index.html](c:\plano\e-vendas\modelo\index.html:643)

Risco:

- `retorno mensal estimado de R$ 3.400,00`
- `3,4% ao mes`
- repeticao do mesmo valor em todos os cenarios

Isso pode soar como promessa ou rendimento predefinido.

Melhoria recomendada:

- trocar `retorno mensal estimado` por `referencia economica da opcao`
- trocar `R$ 3.400,00 por mes` por `cenario de distribuicao mensal de referencia, sujeito a apuracao contratual`
- evitar repetir o mesmo valor em todos os cenarios se ele nao deriva dos cenarios

Texto sugerido:

- `Referencia economica da opcao de R$ 100 mil: distribuicao mensal indicativa de ate R$ 3.400,00, sujeita a desempenho operacional, criterios de apuracao e instrumentos contratuais.`

### 2. Remover ou suavizar termos de garantia forte

Trechos sensiveis:

- [index.html](c:\plano\e-vendas\modelo\index.html:189)
- [index.html](c:\plano\e-vendas\modelo\index.html:258)
- [index.html](c:\plano\e-vendas\modelo\index.html:259)
- [index.html](c:\plano\e-vendas\modelo\index.html:647)

Risco:

- `garantia contratual reforcada`
- `garantia real principal`

Sem instrumento assinado, avaliacao juridica e estrutura operacional implementada, isso pode parecer excesso de seguranca prometida.

Melhoria recomendada:

- usar `mecanismos de protecao contratual propostos`
- usar `estrutura de protecao sugerida`
- usar `recebiveis elegiveis para eventual cessao fiduciaria, sujeitos a validacao juridica e operacional`

Texto sugerido:

- `Estrutura de protecao contratual sugerida, com mecanismos a serem validados na formalizacao.`

### 3. Separar melhor as duas teses: societaria e financeira

Trechos sensiveis:

- [index.html](c:\plano\e-vendas\modelo\index.html:226)
- [index.html](c:\plano\e-vendas\modelo\index.html:353)
- [index.html](c:\plano\e-vendas\modelo\index.html:358)
- [index.html](c:\plano\e-vendas\modelo\index.html:624)
- [index.html](c:\plano\e-vendas\modelo\index.html:641)
- [index.html](c:\plano\e-vendas\modelo\index.html:643)
- [index.html](c:\plano\e-vendas\modelo\index.html:645)

Risco:

- a pagina apresenta `entrada societaria` e `aporte com retorno financeiro` na mesma narrativa, sem separar governanca, risco, direitos economicos e implicacoes juridicas com profundidade suficiente

Melhoria recomendada:

- criar dois blocos visuais independentes:
  - `Opcao A - parceria societaria`
  - `Opcao B - parceria comercial/financeira sujeita a formalizacao`
- cada opcao deve ter:
  - natureza
  - direitos
  - riscos
  - forma de apuracao
  - documentos necessarios

### 4. Evitar sinais de distribuicao publica ampla

Trechos sensiveis:

- [index.html](c:\plano\e-vendas\modelo\index.html:185)
- [index.html](c:\plano\e-vendas\modelo\index.html:661)
- [index.html](c:\plano\e-vendas\modelo\index.html:678)

Risco:

- o material esta pronto para PDF e compartilhamento amplo com linguagem direta de investimento
- isso aumenta a leitura de `oferta ao publico`, especialmente se o arquivo circular livremente

Melhoria recomendada:

- inserir na primeira dobra um aviso de circulacao restrita
- marcar o material como `documento preliminar para analise privada`
- limitar distribuicao a contatos individualizados

Texto sugerido:

- `Material preliminar de uso restrito, compartilhado em contexto privado para discussao exploratoria. Nao constitui oferta publica de valores mobiliarios, nem solicitacao publica de investimento.`

## Prioridade media

### 5. Corrigir termos financeiros para mais precisao

Trechos sensiveis:

- [index.html](c:\plano\e-vendas\modelo\index.html:189)
- [index.html](c:\plano\e-vendas\modelo\index.html:212)
- [index.html](c:\plano\e-vendas\modelo\index.html:213)

Risco:

- `faturamento liquido mensal` mistura conceitos
- faturamento e lucro nao sao a mesma coisa

Melhoria recomendada:

- se o numero de `R$ 10 mil` for lucro, usar `lucro liquido mensal atual`
- se for faturamento, ajustar todo o resto da pagina

Texto sugerido:

- `Lucro liquido mensal atual`

### 6. Revisar nomes que soam promocionais demais

Trechos sensiveis:

- [index.html](c:\plano\e-vendas\modelo\index.html:186)
- [index.html](c:\plano\e-vendas\modelo\index.html:385)
- [index.html](c:\plano\e-vendas\modelo\index.html:428)
- [index.html](c:\plano\e-vendas\modelo\index.html:489)
- [index.html](c:\plano\e-vendas\modelo\index.html:624)

Melhoria recomendada:

- `Plano de Investimento` -> `Memorando Executivo Preliminar`
- `Tres camadas de protecao do investidor` -> `Aspectos de mitigacao e estrutura proposta`
- `Modelo de retorno` -> `Estrutura economica ilustrativa`
- `Leitura comparativa do lucro incremental` -> `Cenarios operacionais ilustrativos`
- `Duas opcoes objetivas de entrada` -> `Alternativas preliminares de estruturacao`

### 7. Suavizar expressao `Parte lucro`

Trecho sensivel:

- [index.html](c:\plano\e-vendas\modelo\index.html:361)

Risco:

- soa informal demais para material serio

Melhoria recomendada:

- usar `Participacao economica`
- ou `Participacao nos resultados`

## Prioridade comercial

### 8. Aumentar confianca com governanca, nao com promessas

Hoje a pagina tenta passar confianca por:

- retorno mensal
- teto
- garantia

Isso ajuda no curto prazo, mas investidores melhores tendem a confiar mais em:

- processo de apuracao
- demonstrativos
- governanca
- direitos de informacao
- cenarios com premissas abertas
- riscos assumidos de forma adulta

Melhorias recomendadas:

- incluir quadro `Como a apuracao sera feita`
- incluir `Premissas do cenario base`
- incluir `Riscos e condicionantes do cenario`
- incluir `Documentos disponiveis em diligencia`

### 9. Trocar certezas por faixas e condicionantes

Exemplos:

- `R$ 3.400,00 por mes` -> `faixa indicativa de distribuicao mensal`
- `atingir o teto em ate 36 meses` -> `horizonte indicativo, sujeito a desempenho, caixa e execucao`
- `desde o mes 1` -> `com possibilidade de inicio na fase inicial, conforme caixa e regras contratuais`

### 10. Dar mais espaco para diligencia

Adicionar uma secao curta:

- balanco e DRE disponiveis sob confidencialidade
- contratos ativos e base de clientes apresentados em diligencia
- metricas operacionais e recorrencia demonstradas em reuniao tecnica

Isso passa maturidade.

## Ajustes de texto sugeridos

### Hero

Atual:

- `Plano de Investimento`
- `retorno estruturado`

Sugestao:

- `Memorando Executivo Preliminar`
- `estrutura economica proposta`

### Bloco de R$ 100 mil

Atual:

- `Retorno mensal estimado`

Sugestao:

- `Referencia economica mensal`

Atual:

- `Retorno em 12 meses`

Sugestao:

- `Projecao anual ilustrativa`

### Seguranca

Atual:

- `Tres camadas de protecao do investidor`

Sugestao:

- `Elementos de mitigacao e suporte contratual`

### Resumo final

Atual:

- `Direito principal: Retorno mensal estimado de R$ 3.400,00`

Sugestao:

- `Referencia economica: distribuicao indicativa mensal, sujeita a apuracao e formalizacao contratual`

## Estrutura recomendada da proxima versao

### Pagina 1

- memorando preliminar
- tese da empresa
- status operacional
- aviso de circulacao restrita

### Pagina 2

- opcao A: parceria societaria
- opcao B: estrutura economica/financeira
- comparativo lado a lado

### Pagina 3

- premissas operacionais
- cenarios
- uso do capital

### Pagina 4

- governanca
- prestacao de contas
- documentos de diligencia
- observacoes juridicas

## Lista objetiva do que mudar no HTML

1. Inserir aviso de uso restrito no topo e no rodape.
2. Trocar `Plano de Investimento` por nome mais neutro.
3. Trocar `retorno mensal estimado` por `referencia economica mensal` nos cards e tabelas.
4. Remover repeticao de `R$ 3.400,00 por mes` como se fosse garantido em todos os cenarios.
5. Trocar `garantia` por `mecanismos de protecao contratual propostos`.
6. Trocar `Parte lucro` por `Participacao nos resultados` ou `Participacao economica`.
7. Corrigir `faturamento liquido mensal` para `lucro liquido mensal atual`, se esse for o dado correto.
8. Reescrever a secao final para separar melhor a opcao societaria da opcao financeira.
9. Incluir secao de premissas e diligencia.
10. Levar a versao revisada para validacao de advogado societario/regulatorio antes de circular amplamente.

## Ordem sugerida de execucao

1. Ajustar nomenclatura e avisos legais leves.
2. Corrigir promessas excessivamente deterministicas.
3. Separar estruturalmente as duas opcoes.
4. Reforcar governanca, diligencia e apuracao.
5. Submeter a versao final a revisao juridica.

