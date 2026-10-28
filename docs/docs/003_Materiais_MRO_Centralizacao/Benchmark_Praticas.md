---
sidebar_position: 6
slug: /mro-centralizacao/benchmark-praticas
title: Benchmark de práticas
description: Referências de gestão de MRO e critérios mensuráveis para avaliar alternativas
---

# Benchmark de práticas

## Objetivo e seleção das referências

O benchmark compara **práticas e mecanismos de gestão**, não o desempenho financeiro de empresas. A pesquisa complementar de **28/10/2026** selecionou três referências primárias: um estudo sucroalcooleiro e duas descrições institucionais de abastecimento industrial.[1–3] Elas cobrem cadastro, reposição e retirada no ponto de uso.

Os critérios de seleção foram relação com MRO, descrição verificável do funcionamento e possibilidade de converter o aprendizado em critério de análise. Fontes comerciais documentam funcionalidades declaradas, sem comprovar economia independente. Não foi verificada a adoção dessas soluções pela São Martinho nem sua disponibilidade contratual para as unidades estudadas.

## Comparação

<p style={{textAlign: 'center'}}>Tabela 1 — Referências, evidências e limites de transferência</p>

| Prática e referência | Contexto e evidência | Benefício observado ou proposto | Risco ou limitação | Aplicação a investigar |
|---|---|---|---|---|
| Cadastro preventivo — Mantovani e Sandrini, UFU [1] | Estudo de compras e cadastro de peças agrícolas em uma usina; identifica o cadastro de peças novas como causa de emergências | Os autores propõem antecipação de cadastros e colaboração técnica de fornecedores; o resumo não demonstra redução após implantação | Uma usina; não prova que a mesma causa predomine em outra empresa | Cadastrar peças antes da entrada de novos equipamentos (hipótese) |
| Reposição gerenciada — Fastenal, FMI [2] | FASTStock verifica e repõe saldos por visitas; FASTBin monitora remotamente; FAST360 mostra posições de estoque | Funcionalidades declaradas podem antecipar reposição e facilitar localização; sem percentual de economia adotado | Dependência de atendimento, integração e qualidade dos dados; fonte comercial | Testar reposição de consumíveis recorrentes com metas contratuais (hipótese) |
| Retirada controlada — Grainger, KeepStock Vending [3] | Folheto descreve acesso por identificação, limites de retirada e relatórios de utilização | Acesso contínuo e rastreabilidade declarados; redução de perdas é alegação sem comprovação independente nesta análise | Compatibilidade e capacidade do equipamento; falhas de autenticação ou máquina; bloqueio indevido em emergência | Testar acesso próximo à manutenção e consumo rastreável com contingência (hipótese) |

<p style={{textAlign: 'center'}}>Fonte: elaboração dos autores a partir de [1–3]. Propostas e alegações comerciais não são resultados medidos.</p>

O estudo da UFU evidencia um gargalo anterior à compra. As duas soluções comerciais tratam disponibilidade e uso, mas pressupõem identificação confiável. O aprendizado conjunto é identificar o material, enxergar saldo utilizável, repor no prazo e registrar a retirada **(inferência)**. Isso pode ocorrer em qualquer [modelo de armazenagem](/mro-centralizacao/modelos-gestao-armazenagem).

Reposição por fornecedor (VMI) define responsabilidade de gestão; consignação define propriedade e pagamento. Uma não implica a outra. Contratos precisam esclarecer inventário, perdas e faturamento. Tecnologia de retirada também não define, por si só, se a rede será centralizada ou local **(distinções analíticas dos autores)**.

## Comparabilidade e limitações

| Dimensão | Limite | Tratamento |
|---|---|---|
| Setor e materiais | Caso de manutenção agrícola versus abastecimento industrial amplo | Validar família de materiais e criticidade antes da transferência |
| Escala e geografia | Não há base comum de distâncias, volumes e unidades | Não transportar custos e prazos para a São Martinho |
| Tecnologia | Plataformas pressupõem infraestrutura e integração | Verificar conectividade, cadastro, suporte e operação em falha |
| Resultados | Ausência de indicador antes/depois padronizado | Comparar mecanismos e medir benefícios em piloto |
| Independência | Duas referências têm interesse comercial | Exigir validação operacional das alegações |

Não há base para classificar uma referência como superior ou atribuir economia específica à companhia. O benchmark revela requisitos e perguntas para análise.

## Critérios de análise {#criterios-de-analise}

A tabela seguinte é uma **proposta dos autores**, derivada do benchmark e dos conflitos discutidos em [modelos de gestão e armazenagem](/mro-centralizacao/modelos-gestao-armazenagem). Metas precisam ser definidas com Manutenção, Operação, Suprimentos e Logística antes da pontuação. Os indicadores ainda não foram medidos na empresa.

<p style={{textAlign: 'center'}}>Tabela 2 — Definições operacionais para comparar configurações</p>

| Critério | Como medir | Dado necessário | Direção e uso |
|---|---|---|---|
| Atendimento no prazo | Requisições atendidas integralmente até o prazo acordado ÷ requisições com vencimento no período × 100; segmentar por criticidade | Quantidade, prazo e entrega ao usuário | Maior é melhor; mínimo obrigatório para críticos |
| Tempo completo | Horas da requisição validada à entrega no ponto de uso; mediana e percentil 95 | Aprovação, separação, expedição, transporte e recebimento | Menor é melhor; P95 evidencia atrasos ocultos pela média |
| Custo total anual | Aquisição, manutenção do estoque, armazéns, frete, sistemas, perdas e faltas; implantação separada | Custos na mesma base e hipóteses de faltas | Menor é melhor, após cumprir restrições |
| Capital em estoque | Estoque médio valorizado ao mesmo custo unitário, em todos os níveis | Saldos locais e centrais; propriedade contratual | Menor para serviço equivalente; não confundir propriedade com redução física |
| Resiliência | Simular falha de centro, rota ou fornecedor; contar demandas críticas não atendidas no prazo | Rotas alternativas, reservas e contingência | Menor exposição é melhor; cobertura mínima pode ser eliminatória |
| Qualidade do cadastro | Itens candidatos com especificação, código coerente e equivalência validada ÷ candidatos × 100 | Cadastro e homologação técnica | Maior é melhor; incompatibilidade impede compartilhar o item |
| Acuracidade | Posições item/local com quantidade física igual à registrada ÷ posições contadas × 100 | Contagem com método e amostra constantes | Maior é melhor; separar erros em críticos |
| Viabilidade de execução | Evidências de preservação, capacidade, conectividade, integração, equipe, contrato e contingência | Checklist com responsável por requisito | Requisito obrigatório descumprido elimina alternativa |

<p style={{textAlign: 'center'}}>Fonte: elaboração dos autores (2026). Definições propostas, sem resultados reais da companhia.</p>

### Regras para avaliação

1. **Fixar o recorte:** mesma lista de materiais, demanda, calendário e horizonte para todas as alternativas; separar safra, entressafra e unidades.
2. **Aplicar restrições antes dos pesos:** se uma peça crítica tolera espera menor que a transferência confiável, e não existe proteção local, a configuração é inviável para esse item. Economia não compensa essa restrição.
3. **Fixar escalas previamente:** em critério crescente, nota 1 no limite inferior e 5 na meta superior, interpolação linear e valores limitados entre 1 e 5. Inverter para custo e tempo. Justificar os limites. Dado ausente é pendência, não nota intermediária.
4. **Evitar dupla contagem:** tempo e serviço são correlacionados; capital já pode aparecer no custo de manutenção. Usar indicadores como diagnóstico ou repartir seu peso explicitamente, sem somar o mesmo benefício duas vezes.
5. **Validar pesos:** soma de 100%, justificativa e responsáveis. Não inventar prioridades da companhia sem consulta. A aplicação numérica em cenário genérico está reservada à [matriz multicritério](/mro-centralizacao/matriz-decisao-multicriterio), fora destas duas tarefas.
6. **Testar sensibilidade:** variar pesos e hipóteses de frete, atraso e demanda de pico. Registrar quando muda a classificação; resultado instável pede evidência adicional.

## Aprendizados transferíveis e validação

Em cenário genérico, um piloto poderia começar por consumíveis padronizados **(hipótese)**. Medir a situação inicial, comparar períodos de demanda equivalente, separar implantação de custo recorrente e acompanhar atendimento, faltas, acuracidade e trabalho de reposição. Menos retiradas não comprovam eficiência sem verificar falta de material ou mudança da produção.

Definir previamente metas, contingência e condições de interrupção do piloto. Não há base para estabelecer metas numéricas reais nesta pesquisa. Um resultado favorável em consumíveis não autoriza expansão automática a sobressalentes críticos.

Para a São Martinho, cadastro comum, reposição monitorada e retirada rastreável são **hipóteses de investigação**, não diagnóstico de falhas. Permanecem lacunas sobre sistemas em uso, contratos, custos, acuracidade, metas e resultados por categoria. As referências ajudam a estruturar a coleta necessária à decisão.

## Fontes

1. MANTOVANI, Carol; SANDRINI, João Pedro Bruno. *Planejamento do cadastro de peças de manutenção: um estudo de caso em uma usina sucroalcooleira*. TCC, Universidade Federal de Uberlândia, defesa em 16 mar. 2020. [Registro e resumo institucional](https://repositorio.ufu.br/handle/123456789/29263). Acesso em: 28 out. 2026. O registro apresenta 2019 na descrição bibliográfica e 2020 na defesa; foi utilizado o resumo, sem afirmar implantação das propostas.
2. FASTENAL. *Fastenal Managed Inventory 101*. The Blue Print, atualização em 21 fev. 2025. [Descrição institucional de FMI](https://blueprint.fastenal.com/fmi-technology-101.html). Acesso em: 28 out. 2026. Fonte comercial; funcionalidades declaradas pelo fornecedor.
3. GRAINGER. *KeepStock Vending*. Folheto institucional, s. d. [Funcionamento e controles](https://grainger-prod.adobecqms.net/content/dam/grainger/gus/en/public/marketing-material/flyer/W-CTKS174_SS-KS-VEND_Collateral_FL_FF.pdf). Acesso em: 28 out. 2026. Fonte comercial, sem data editorial indicada no documento consultado.
