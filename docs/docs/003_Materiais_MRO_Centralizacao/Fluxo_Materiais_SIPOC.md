---
sidebar_position: 4
slug: /mro-centralizacao/fluxo-materiais-sipoc
title: Fluxo de materiais e SIPOC
description: Mapeamento do fluxo da necessidade à entrega na São Martinho
---

# Fluxo de materiais e SIPOC

## Escopo do processo

O mapa descreve o caminho de um material MRO desde o momento em que a manutenção ou a operação percebe que precisa dele até o momento em que ele chega às mãos de quem vai usá-lo. A ferramenta escolhida foi o SIPOC (*Suppliers, Inputs, Process, Outputs, Customers*), uma técnica de mapeamento de alto nível que organiza o processo em fornecedores, entradas, etapas, saídas e clientes. Ela ajuda a visualizar interfaces, dependências e possíveis pontos de retrabalho entre as áreas envolvidas, o que é útil em um fluxo que atravessa manutenção, almoxarifado, suprimentos, aprovadores e fornecedores.<sup>[2](#ref2)</sup> <sup>[5](#ref5)</sup> <sup>[6](#ref6)</sup> <sup>[14](#ref14)</sup>

- **Evento inicial:** identificação da necessidade de material MRO por manutenção, operação agrícola, operação industrial ou outra área usuária da São Martinho, a partir de uma ordem de serviço (preventiva, preditiva ou corretiva), e emissão da requisição.
- **Evento final:** entrega do material ao solicitante, com recebimento, conferência, baixa no estoque e disponibilização para uso na ordem de serviço ou na operação.
- **Unidade de análise:** a requisição de um item MRO (código de material, quantidade, prioridade e data necessária), considerando o fluxo interno de suprimento entre manutenção, almoxarifado, compras, fornecedores e logística. O mapa cobre os dois caminhos possíveis: o do item disponível em estoque e o do item que precisa ser reposto por compra ou por transferência entre unidades.
- **Premissas do cenário:**
  - O mapa representa um fluxo genérico aplicável ao contexto da São Martinho, que opera atividades agrícolas, usinas, moendas, cogeração e produção de açúcar e etanol.<sup>[3](#ref3)</sup> Ele não descreve obrigatoriamente o processo real da companhia, que deve ser confirmado com documentos internos e entrevistas.
  - Cada unidade possui almoxarifado próprio, e a gestão ocorre em um sistema integrado (ERP) com cadastro de materiais, saldos, reservas, pedidos e ordens de serviço.
  - Os itens possuem classificação por Curva ABC e por criticidade, e a compra segue alçadas de aprovação.
  - A demanda varia entre a safra, em que a reposição ocorre com o equipamento em uso, e a entressafra, em que tendem a se concentrar as paradas programadas.
  - O mapa descreve o processo como ele deve funcionar, e não mede tempos, custos ou volumes.

## SIPOC

A estrutura parte dos fornecedores e termina nos clientes, o que permite identificar quem fornece cada insumo, quais recursos entram no processo, quais atividades os transformam e quem recebe o resultado.<sup>[2](#ref2)</sup> <sup>[5](#ref5)</sup> <sup>[14](#ref14)</sup>

| Suppliers — Fornecedores | Inputs — Entradas | Process — Processo | Outputs — Saídas | Customers — Clientes |
|---|---|---|---|---|
| Áreas usuárias: manutenção mecânica, elétrica, automação, agrícola e industrial | Necessidade de material; descrição técnica; quantidade; urgência; vínculo com ordem de serviço ou equipamento; lista de materiais do plano de manutenção | 1. Identificar a necessidade e emitir a requisição | Requisição de material registrada, com código, quantidade, prioridade e data necessária | Almoxarifado; planejamento de materiais |
| Almoxarifado; sistema de gestão (ERP) | Requisição; saldo físico e do sistema; reservas existentes; localização no estoque | 2. Verificar a disponibilidade e reservar o material | Reserva do material ou registro de indisponibilidade | Solicitante; planejamento de materiais e compras, quando não há saldo |
| Planejamento de materiais; controladoria | Histórico de consumo; parâmetros de reposição (mínimo e máximo); classificação ABC e criticidade; custo; lead time cadastrado; calendário de safra e entressafra | 3. Planejar a reposição e definir a forma de atendimento (estoque, compra ou transferência) | Decisão de atendimento e solicitação de compra ou de transferência | Aprovadores; compras |
| Gestores da área solicitante; suprimentos; controladoria | Solicitação; centro de custo e orçamento; justificativa técnica; criticidade e impacto operacional da falta | 4. Aprovar a solicitação conforme a alçada | Solicitação aprovada, devolvida ou recusada | Compras |
| Compras; fornecedores homologados; outras unidades | Especificação técnica; cotações; prazo de entrega; condições comerciais; certificados, quando aplicáveis; saldo em outras unidades | 5. Cotar, selecionar o fornecedor e emitir o pedido de compra ou a ordem de transferência | Pedido emitido e confirmado, com preço, prazo e condições | Fornecedor; almoxarifado; solicitante |
| Fornecedores; transportadoras e logística | Pedido; programação de entrega; nota fiscal; romaneio; condições de transporte | 6. Acompanhar a entrega e transportar o material | Material em trânsito, com previsão de chegada atualizada | Recebimento; compras |
| Transportadoras; fornecedores | Material físico; nota fiscal; romaneio; pedido; especificação e documentos técnicos | 7. Receber, conferir e inspecionar | Entrada física e fiscal registrada; material liberado ou recusado | Almoxarifado; controle de qualidade; área fiscal |
| Recebimento; cadastro de materiais | Material liberado; endereço de armazenagem; condições de guarda (validade e embalagem) | 8. Armazenar e endereçar o material | Saldo atualizado no sistema; item localizável; reserva vinculada à requisição, se houver | Almoxarifado; manutenção; planejamento de materiais |
| Almoxarifado; manutenção | Requisição aprovada; saldo disponível; localização no estoque; documento de retirada | 9. Separar, entregar ao usuário e dar baixa | Material entregue ao solicitante; estoque atualizado; consumo apontado na ordem de serviço | Manutenção; operação agrícola e industrial; planejamento de materiais (o consumo alimenta o histórico) |

## Detalhamento do fluxo

**Solicitação.** A necessidade surge quando uma ordem de manutenção preventiva, preditiva ou corretiva exige um material, ou quando a operação agrícola ou industrial identifica a reposição de um item. Nas preventivas e preditivas, a lista de materiais já está prevista no plano e a requisição pode ser antecipada; nas corretivas, ela nasce de uma falha, com urgência e menos informação sobre o item. A requisição é o pedido formal do setor consumidor ao almoxarifado e deve conter descrição técnica, quantidade, equipamento de destino, urgência e, quando possível, o código do material cadastrado.<sup>[12](#ref12)</sup> A qualidade dessa informação determina a qualidade do restante do fluxo, porque um cadastro ruim ou uma prioridade mal informada se propagam para a reserva, a compra e a entrega.<sup>[1](#ref1)</sup>

**Planejamento e verificação de estoque.** O almoxarifado ou a área de planejamento verifica se existe saldo disponível, se o item está reservado para outra ordem e se os parâmetros de reposição estão adequados, além de conferir se a requisição segue os padrões definidos e se a quantidade é compatível com a disponibilidade.<sup>[12](#ref12)</sup> Havendo saldo, o material é reservado e o fluxo salta para a entrega, que é o caminho mais curto e o que a política de estoque busca viabilizar. Não havendo, a demanda segue para o planejamento, que decide entre usar o estoque de outra unidade, quando isso for possível, ou comprar, ponderando o lead time esperado, a criticidade do item, a época do ano e a existência de contrato ou fornecedor homologado.<sup>[7](#ref7)</sup> <sup>[8](#ref8)</sup>

**Aprovação.** Conforme o valor, a criticidade e a política interna, a requisição pode exigir aprovação do gestor solicitante, da manutenção, de suprimentos ou da controladoria. A análise deve considerar a necessidade técnica, o impacto operacional da falta e o custo total, incluindo não apenas o preço do material, mas também o risco de indisponibilidade.<sup>[1](#ref1)</sup> <sup>[8](#ref8)</sup> <sup>[9](#ref9)</sup> A aprovação é uma etapa de controle, mas também uma fonte de espera, sobretudo quando a necessidade é urgente.

**Compra ou separação.** Se há estoque, o fluxo segue para separação e entrega. Se não há saldo, a demanda é encaminhada para cotação e compra. O processo típico envolve o recebimento da requisição aprovada, a seleção de fornecedores, o envio da solicitação de cotação, a análise de preços, prazos e condições e a emissão da ordem de compra.<sup>[13](#ref13)</sup> Quando o atendimento se dá por transferência entre unidades, o equivalente é a ordem de transferência, que também exige confirmação de saldo, separação e transporte.

**Transporte e recebimento.** Emitido o pedido, o fornecedor ou a transportadora entrega o material à unidade, e o prazo prometido deve ser acompanhado, já que o lead time efetivamente praticado costuma diferir do informado.<sup>[7](#ref7)</sup> <sup>[8](#ref8)</sup> O recebimento confere quantidade, especificação, estado de conservação, nota fiscal e documentos técnicos exigidos. Recebimento, controle e liberação de materiais integram o fluxo de aquisição e administração de materiais dentro da cadeia de suprimentos, e divergências nessa etapa geram devolução, reposição ou retrabalho.<sup>[10](#ref10)</sup> <sup>[11](#ref11)</sup>

**Armazenagem e entrega ao usuário.** O material liberado é armazenado e endereçado, o que atualiza o saldo e permite que seja localizado; se havia reserva para uma ordem específica, ela é vinculada ao item recebido. Em seguida, o almoxarifado separa o material, entrega ao solicitante e dá a baixa. A entrega deve estar vinculada à requisição e, quando aplicável, à ordem de serviço, com registro de data e do setor que recebeu.<sup>[12](#ref12)</sup> Esse vínculo permite rastrear o consumo, avaliar giro, identificar itens sem movimento e melhorar os parâmetros de reposição, fechando o ciclo de informação.<sup>[1](#ref1)</sup> <sup>[4](#ref4)</sup>

O processo é, na prática, dois fluxos em um: um **fluxo curto** (solicitação, verificação, reserva e entrega) para o item em estoque e um **fluxo longo** (que inclui planejamento, aprovação, compra, transporte, recebimento e armazenagem) para o item sem saldo. A proporção de requisições que segue cada caminho é um bom retrato da política de estoque: quanto mais requisições precisam do fluxo longo, mais o processo depende de compras e menor tende a ser o nível de serviço do almoxarifado.<sup>[1](#ref1)</sup> <sup>[4](#ref4)</sup>

## Pontos de controle e riscos

| Etapa | Responsável | Informação necessária | Risco | Controle ou indicador |
|---|---|---|---|---|
| 1. Identificação da necessidade e requisição | Manutenção, operação agrícola ou operação industrial | Descrição técnica, quantidade, equipamento, urgência e ordem de serviço | Requisição incompleta, com especificação errada ou emitida tarde em relação ao plano da parada | Percentual de requisições devolvidas; retrabalho de cadastro; antecedência da requisição; tempo de tratamento da solicitação |
| 2. Verificação de estoque e reserva | Almoxarifado e planejamento | Saldo disponível, reservas, localização e parâmetros de reposição | Atendimento incorreto por saldo desatualizado ou material reservado para outra ordem | Acuracidade de inventário; divergências de saldo; itens sem movimento; percentual de requisições sem saldo<sup>[4](#ref4)</sup> <sup>[8](#ref8)</sup> |
| 3. Planejamento da reposição | Planejamento de materiais | Histórico de consumo, parâmetros, ABC e criticidade, lead time real e plano de paradas | Parâmetros desatualizados; lead time subestimado; decisão sem considerar a criticidade | Taxa de ruptura de itens críticos; diferença entre lead time cadastrado e real; revisão de parâmetros<sup>[7](#ref7)</sup> <sup>[8](#ref8)</sup> <sup>[9](#ref9)</sup> |
| 4. Aprovação | Gestor solicitante, suprimentos e controladoria | Valor, criticidade, justificativa técnica e impacto operacional | Atraso de aprovação em item crítico ou aprovação sem análise adequada | Tempo médio de aprovação; requisições atrasadas; compras emergenciais<sup>[1](#ref1)</sup> <sup>[8](#ref8)</sup> |
| 5. Cotação e compra | Compras | Especificação, quantidade, prazo, condições comerciais e fornecedores alternativos | Fornecedor com prazo longo, preço elevado ou indisponibilidade; compra duplicada por cadastro duplicado | Lead time de compra; aderência ao prazo; número de fornecedores por item crítico<sup>[13](#ref13)</sup> |
| 6. Acompanhamento e transporte | Compras; fornecedor; transportadora | Prazo prometido, programação de entrega e rastreamento | Atraso não informado; avaria no transporte; atraso crítico às vésperas da entressafra | Lead time real por fornecedor; percentual de entregas no prazo; pedidos críticos em atraso<sup>[7](#ref7)</sup> <sup>[8](#ref8)</sup> |
| 7. Recebimento e inspeção | Almoxarifado e controle de qualidade | Nota fiscal, romaneio, quantidade, especificação e documentos técnicos | Recebimento de material divergente, danificado ou fora de especificação; acúmulo de recebimentos em períodos de pico | Taxa de divergência no recebimento; devoluções; tempo de inspeção<sup>[10](#ref10)</sup> <sup>[12](#ref12)</sup> |
| 8. Armazenagem e endereçamento | Almoxarifado | Endereço, validade, condições de guarda e vínculo com a reserva | Item guardado em local errado ou sem registro; vencimento ou deterioração; obsolescência não percebida | Acuracidade de inventário; itens com validade próxima; valor de itens sem movimento<sup>[4](#ref4)</sup> <sup>[8](#ref8)</sup> |
| 9. Separação e entrega | Almoxarifado | Requisição aprovada, saldo, localização e destinatário | Atraso na separação, erro de item ou baixa incorreta do estoque | Tempo de atendimento; taxa de erro na separação; requisições pendentes<sup>[12](#ref12)</sup> |
| 10. Consumo e retorno de informação | Manutenção e almoxarifado | Material utilizado, ordem de serviço, equipamento e data de uso | Falta de rastreabilidade; baixa em ordem de serviço errada; parâmetros de reposição desatualizados | Giro de estoque; cobertura em dias; taxa de ruptura; compras emergenciais<sup>[1](#ref1)</sup> <sup>[4](#ref4)</sup> <sup>[8](#ref8)</sup> |

## Aprendizados

O fluxo evidencia que a entrega de material não depende apenas do almoxarifado: envolve manutenção, operação, planejamento, compras, fornecedores, logística e controladoria. A principal dependência é a qualidade da informação na solicitação, pois erro de especificação ou ausência de vínculo com a ordem de serviço compromete todas as etapas seguintes.<sup>[1](#ref1)</sup> <sup>[4](#ref4)</sup> Os pontos abaixo são hipóteses a investigar, e não diagnósticos, já que o cenário é genérico e não se apoia em medições do processo real.

Os principais gargalos potenciais são:

- **Verificação de estoque desatualizada**, que pode gerar compra desnecessária ou falsa sensação de disponibilidade, e que, no caso contrário, aciona o fluxo longo sem necessidade.<sup>[4](#ref4)</sup>
- **Aprovação lenta**, especialmente em itens críticos, podendo transformar uma necessidade planejada em compra emergencial.<sup>[1](#ref1)</sup> <sup>[8](#ref8)</sup>
- **Lead time longo ou variável**, que exige estoque de segurança, contratos de fornecimento ou qualificação de fornecedores alternativos.<sup>[7](#ref7)</sup> <sup>[8](#ref8)</sup>
- **Recebimento sem conferência adequada ou em pico de volume**, que pode liberar material fora de especificação e gerar parada posterior.<sup>[10](#ref10)</sup> <sup>[12](#ref12)</sup>
- **Falta de rastreabilidade entre requisição, ordem de serviço e consumo**, o que dificulta calcular giro, cobertura e nível de serviço.<sup>[1](#ref1)</sup> <sup>[4](#ref4)</sup>

No contexto da São Martinho, a sazonalidade da safra e a diversidade de ativos (agrícolas, industriais, de transporte e de cogeração) aumentam a importância de classificar materiais por criticidade e de monitorar compras emergenciais, rupturas e tempo de atendimento.<sup>[3](#ref3)</sup> <sup>[9](#ref9)</sup> Entre as perguntas que o mapa deixa em aberto estão: quanto tempo cada etapa consome de fato e qual parcela do tempo total é espera; que proporção das requisições segue o fluxo curto e que proporção segue o longo; quais motivos dominam as compras emergenciais; como o tempo de aprovação varia entre classes e criticidades; qual é a diferença entre o lead time cadastrado e o praticado, por fornecedor; e em que categorias de material se concentram as divergências de recebimento e de saldo. O mapa não constitui uma proposta de centralização ou de reorganização do processo real; ele serve como base para investigar onde o fluxo apresenta atrasos, retrabalhos e riscos de indisponibilidade.

---

## Fontes

1. <a id="ref1"></a>UNIVERSIDADE ESTADUAL DE PONTA GROSSA. Análise do nível de serviço e custo de estoques MRO. *Revista de Administração do Paraná*, Ponta Grossa, [s. d.]. Disponível em: [https://revistas.uepg.br/index.php/admpg/article/download/14082/209209211202/](https://revistas.uepg.br/index.php/admpg/article/download/14082/209209211202/). Acesso em: 27 out. 2026.

2. <a id="ref2"></a>ASANA. O que é um diagrama SIPOC? 7 etapas para mapear processos. [S. l.], 16 mar. 2026. Disponível em: [https://asana.com/pt/resources/sipoc-diagram](https://asana.com/pt/resources/sipoc-diagram). Acesso em: 27 out. 2026.

3. <a id="ref3"></a>EU QUERO INVESTIR. São Martinho encerra safra 2025/26 com lucro de R$ 836 milhões. [S. l.], 2026. Disponível em: [https://euqueroinvestir.com/acoes/sao-martinho-encerra-safra-2025-26-com-lucro-de-r-836-milhoes](https://euqueroinvestir.com/acoes/sao-martinho-encerra-safra-2025-26-com-lucro-de-r-836-milhoes). Acesso em: 27 out. 2026.

4. <a id="ref4"></a>UNIVERSIDADE DE SÃO PAULO. Gestão de estoques de manutenção, reparo e operação. São Paulo, [s. d.]. Disponível em: [https://bdta.abcd.usp.br/directbitstream/ef939129-e32d-4225-8052-051c22969cf4/EQ19042%20(1)%20Daphine.pdf](https://bdta.abcd.usp.br/directbitstream/ef939129-e32d-4225-8052-051c22969cf4/EQ19042%20(1)%20Daphine.pdf). Acesso em: 27 out. 2026.

5. <a id="ref5"></a>AMORIM, M. de J.; MANTEGAZINI, D. Z.; XAVIER, T. P.; NICO FILHO, G. H. Aplicação da ferramenta SIPOC no mapeamento de processos de uma cooperativa escolar. 2024. Disponível em: [https://periodicos.ufsm.br/rgc/article/download/87309/65378/432065](https://periodicos.ufsm.br/rgc/article/download/87309/65378/432065). Acesso em: 27 out. 2026.

6. <a id="ref6"></a>TEIXEIRA, A. L. A. Mapeamento de processos: teoria e caso ilustrativo. Rio de Janeiro: Pontifícia Universidade Católica do Rio de Janeiro, 2013. Disponível em: [https://www.puc-rio.br/ensinopesq/ccpg/pibic/relatorio_resumo2013/relatorios_pdf/ctc/IND/IND-AnaLuisaAlvesTeixeira.pdf](https://www.puc-rio.br/ensinopesq/ccpg/pibic/relatorio_resumo2013/relatorios_pdf/ctc/IND/IND-AnaLuisaAlvesTeixeira.pdf). Acesso em: 27 out. 2026.

7. <a id="ref7"></a>SEMANTICS SCHOLAR. Ponto de ressuprimento para materiais com demanda. [S. l.], [s. d.]. Disponível em: [https://pdfs.semanticscholar.org/94c9/90ff16f9586d64c63592bb512d4042f4cf4b.pdf](https://pdfs.semanticscholar.org/94c9/90ff16f9586d64c63592bb512d4042f4cf4b.pdf). Acesso em: 27 out. 2026.

8. <a id="ref8"></a>SISMETRO. Estoque MRO. [S. l.], 2026. Disponível em: [https://sismetro.com/guia/glossario/estoque-mro/](https://sismetro.com/guia/glossario/estoque-mro/). Acesso em: 27 out. 2026.

9. <a id="ref9"></a>SCIELO. Matriz de posicionamento estratégico de materiais. *Gestão & Produção*, [S. l.], [s. d.]. Disponível em: [https://www.scielo.br/j/gp/a/tjmKyH6XY6WSkgwhg4hdZhd/?format=pdf&lang=pt](https://www.scielo.br/j/gp/a/tjmKyH6XY6WSkgwhg4hdZhd/?format=pdf&lang=pt). Acesso em: 27 out. 2026.

10. <a id="ref10"></a>ASSOCIAÇÃO BRASILEIRA DE METALURGIA, MATERIAIS E MINERAÇÃO. Sistemática de recebimento, controle e liberação de materiais na Companhia Siderúrgica Nacional. [S. l.], [s. d.]. Disponível em: [https://abmproceedings.com.br/en/article/download-pdf/sistemtica-de-recebimento-controle-e-liberao-de-materiais-na-companhia-siderurgica-nacional](https://abmproceedings.com.br/en/article/download-pdf/sistemtica-de-recebimento-controle-e-liberao-de-materiais-na-companhia-siderurgica-nacional). Acesso em: 27 out. 2026.

11. <a id="ref11"></a>COGNA EDUCAÇÃO. Gestão de suprimentos: a gestão logística na construção civil. [S. l.], [s. d.]. Disponível em: [https://repositorio.pgsscogna.com.br/bitstream/123456789/49938/1/Adrielly_soares.pdf](https://repositorio.pgsscogna.com.br/bitstream/123456789/49938/1/Adrielly_soares.pdf). Acesso em: 27 out. 2026.

12. <a id="ref12"></a>PREFEITURA MUNICIPAL DE CUITÉ. Manual do almoxarifado. Cuité, 2026. Disponível em: [https://cuite.pb.gov.br/wp-content/uploads/2026/03/MANUAL-DO-ALMOXARIFADOMANUAL%20DO%20ALMOXARIFADO.pdf](https://cuite.pb.gov.br/wp-content/uploads/2026/03/MANUAL-DO-ALMOXARIFADOMANUAL%20DO%20ALMOXARIFADO.pdf). Acesso em: 27 out. 2026.

13. <a id="ref13"></a>UNIVERSIDADE FEDERAL DE VIÇOSA. A importância da cadeia de suprimentos em uma empresa. Viçosa, 2013. Disponível em: [https://saepro.ufv.br/wp-content/uploads/2015/06/2013.6.pdf](https://saepro.ufv.br/wp-content/uploads/2015/06/2013.6.pdf). Acesso em: 27 out. 2026.

14. <a id="ref14"></a>LUCIDCHART. SIPOC: o que é, vantagens e como fazer. [S. l.], 17 jan. 2024. Disponível em: [https://lucid.co/pt/blog/o-que-e-sipoc](https://lucid.co/pt/blog/o-que-e-sipoc). Acesso em: 27 out. 2026.