---
sidebar_position: 3
slug: /mro-centralizacao/modelos-gestao-armazenagem
title: Modelos de gestão e armazenagem
description: Comparação dos modelos de estoque MRO, condições de aplicação e riscos
---

# Modelos de gestão e armazenagem

## Síntese executiva e escopo

Centralizar permite compartilhar materiais, mas pode aumentar o tempo até o equipamento que precisa da peça. Estoques locais encurtam esse percurso, porém podem multiplicar reservas e estruturas. O híbrido combina os mecanismos e exige regras claras de alocação **(inferência)**. A escolha deve considerar famílias de materiais e criticidade, preservando a continuidade operacional.

Esta análise é conceitual, com pesquisa complementar em **28/10/2026**. O contexto público da São Martinho está documentado na [retomada do contexto](/mro-centralizacao/retomada-contexto). Não dispomos de dados internos suficientes para identificar seu modelo atual ou dimensionar uma configuração recomendada. Os exemplos são **hipotéticos**.

## Síntese visual para apresentação

<figure style={{margin: '1.5rem 0'}}>
  <div style={{display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(min(100%, 220px), 1fr))', gap: '1rem'}}>
    <div style={{border: '2px solid var(--ifm-color-primary)', borderRadius: '12px', padding: '1rem'}}>
      <h3>Centralizado</h3>
      <p style={{fontSize: '1.15rem', fontWeight: 700}}>Centro → Unidades</p>
      <p>Uma reserva compartilhada abastece a rede.</p>
      <p><strong>Potencial:</strong> reduzir duplicações.</p>
      <p><strong>Condição:</strong> a transferência precisa caber no prazo tolerável.</p>
    </div>
    <div style={{border: '2px solid var(--ifm-color-primary)', borderRadius: '12px', padding: '1rem'}}>
      <h3>Descentralizado</h3>
      <p style={{fontSize: '1.15rem', fontWeight: 700}}>Reserva em cada unidade</p>
      <p>O atendimento depende do saldo disponível no local.</p>
      <p><strong>Potencial:</strong> resposta próxima à operação.</p>
      <p><strong>Condição:</strong> controlar duplicações e ociosidade.</p>
    </div>
    <div style={{border: '2px solid var(--ifm-color-primary)', borderRadius: '12px', padding: '1rem'}}>
      <h3>Híbrido</h3>
      <p style={{fontSize: '1.15rem', fontWeight: 700}}>Proteção local + reserva comum</p>
      <p>A localização varia conforme o perfil do material.</p>
      <p><strong>Potencial:</strong> combinar acesso e compartilhamento.</p>
      <p><strong>Condição:</strong> coordenar os dois níveis para evitar excesso.</p>
    </div>
  </div>
  <figcaption style={{marginTop: '0.75rem', fontSize: '0.9rem'}}>Figura 1 — Síntese conceitual dos autores, baseada em [1–3]. Não representa a configuração atual da São Martinho.</figcaption>
</figure>

:::tip Roteiro de decisão
**1. Classificar o material → 2. Validar prazo e continuidade → 3. Comparar custo total → 4. Testar contingências.** A alternativa de menor custo só avança se atender às restrições operacionais. Ver [benchmark e resultados publicados](/mro-centralizacao/benchmark-praticas#casos-com-resultados-quantitativos-publicados).
:::

## Três decisões diferentes

| Dimensão | Decisão | Exemplo hipotético |
|---|---|---|
| Compras | Quem negocia e contrata | Contrato corporativo com entrega direta nas usinas |
| Gestão | Quem define cadastro, políticas e prioridades | Cadastro único e metas comuns com execução local |
| Armazenagem física | Onde o material permanece | Reserva compartilhada e peças críticas nas unidades |

Fonte: estrutura analítica dos autores. Compras centralizadas não comprovam estoque físico central. Visibilidade conjunta também não significa disponibilidade para transferência: o saldo pode estar reservado para manutenção.

## Comparação dos modelos

<p style={{textAlign: 'center'}}>Tabela 1 — Alternativas de armazenagem física de MRO</p>

| Modelo | Funcionamento | Benefícios potenciais | Riscos e limitações | Contextos favoráveis |
|---|---|---|---|---|
| Centralizado | Um centro mantém a reserva e abastece as unidades | Compartilhamento de itens comuns; menor duplicação de reservas; concentração de competências de preservação | Transporte até o usuário; dependência do centro e das rotas; disputa pelo mesmo saldo | Itens intercambiáveis, demanda não totalmente simultânea e prazo de transferência compatível |
| Descentralizado | Cada unidade mantém sua reserva | Acesso local, autonomia e menor dependência de transferências | Duplicação de reservas e estruturas; sobra em uma unidade enquanto outra tem falta | Unidades distantes, itens específicos e resposta imediata à manutenção |
| Híbrido | Reserva local selecionada e reserva compartilhada | Combina proteção local e compartilhamento por perfil de item | Pode duplicar estoques sem reduzir o central; exige regras de reposição e prioridade | Rede heterogênea com capacidade de coordenar vários níveis de estoque |

<p style={{textAlign: 'center'}}>Fonte: elaboração dos autores, com base nos mecanismos e limites discutidos em [1–3]. São tendências condicionais, não resultados medidos na São Martinho.</p>

## Dimensões para comparação

| Dimensão | Centralizado | Descentralizado | Híbrido |
|---|---|---|---|
| Serviço e tempo | Depende de separação, expedição e transporte | Atendimento rápido quando existe saldo local | Resposta local para itens selecionados; transferência para os demais |
| Capital imobilizado | Pode reduzir reservas repetidas de itens comuns | Pode exigir reserva em cada unidade | Só reduz capital se os parâmetros dos dois níveis forem revistos juntos |
| Transporte | Acrescenta distribuição do centro às unidades | Pode receber diretamente do fornecedor | Combina rotas regulares e exceções urgentes |
| Governança | Precisa arbitrar prioridade entre unidades | Precisa garantir adesão local à política comum | Precisa definir quem repõe cada nível e autoriza transferências |
| Escala | Pode consolidar recebimento e armazenagem | Estruturas locais podem se repetir | Economia depende das estruturas mantidas |
| Risco de parada | Falha do centro ou rota pode afetar várias unidades | Distribui a exposição, mas não elimina faltas locais | Pode proteger críticos localmente, se a seleção for correta |

Fonte: interpretação dos autores **(inferência)** a partir de [1–3]. Escala de negociação pode existir nos três modelos, independentemente da localização física.

### Compartilhamento e demanda simultânea

O MIT apresenta a agregação de incertezas de demanda como mecanismo de compartilhamento de estoques.[1] A vantagem depende das hipóteses: necessidades simultâneas reduzem a compensação entre sobra e falta. Demandas com eventos extremos também limitam o ganho.[2] Paradas programadas coincidentes entre usinas podem gerar picos simultâneos **(hipótese)**; por isso, a análise deve separar safra e entressafra.

**Exemplo didático:** quatro unidades têm, cada uma, 10 peças de estoque de segurança do mesmo item. Com demandas independentes, variabilidades e prazos iguais e mesmo nível de serviço, a regra simplificada da raiz quadrada estimaria 40 × √(1/4) = **20 peças** em um único local.[1] A redução teórica de **50% é apenas da parcela de segurança**. Não estima o estoque total nem inclui transporte adicional; não é uma economia projetada para a São Martinho. Correlação entre demandas ou aumento do prazo altera o resultado.

### Custo versus atendimento e resiliência

Para comparar alternativas, os autores propõem a mesma demanda, horizonte anual e meta de serviço, usando:

**Custo anual comparável = aquisição + manutenção do estoque + operação dos armazéns + transporte + sistemas e coordenação + perdas e obsolescência + custo esperado das faltas.**

Separar implantação de despesas recorrentes. Estimar faltas por cenários de probabilidade e consequência, com premissas explícitas. Não contar a mesma perda em mais de uma parcela. A concentração pode diminuir reservas e aumentar exposição a interrupções; Schmitt e coautores demonstram esse conflito em modelos com falhas de suprimento.[3] Isso não estabelece superioridade universal da descentralização.

## Segmentação e controles de armazenagem

<p style={{textAlign: 'center'}}>Tabela 2 — Hipóteses a testar por família de materiais</p>

| Perfil | Alternativa a testar | Condição necessária | Controle físico |
|---|---|---|---|
| Peça crítica, sem substituto, com tolerância curta à falta | Reserva local | Manutenção validar criticidade e proteção necessária | Identificação do ativo, preservação e acesso em plantão |
| Sobressalente caro, raro e comum | Reserva compartilhada | Compatibilidade comprovada e transferência no prazo tolerável | Inspeção, conservação e prioridade para falhas simultâneas |
| Consumível recorrente e padronizado | Reposição local por fornecedor ou centro com rota regular | Consumo e prazo conhecidos | Endereçamento, registro de retirada e contagem cíclica |
| Kit de parada programada | Compra planejada e separação por ordem | Cronograma e conferência antes da parada | Reserva identificada, controle de faltas no kit e devolução das sobras |
| Item com validade ou conservação especial | Local tecnicamente habilitado | Respeitar especificação e ficha de segurança aplicável | Controle de lote, validade e ambiente; saída pela validade mais próxima quando aplicável |

<p style={{textAlign: 'center'}}>Fonte: propostas dos autores (hipóteses), sem classificação dos materiais reais da empresa.</p>

ABC financeira não substitui criticidade: uma peça barata pode interromper um ativo essencial. O saldo utilizável deve excluir itens vencidos, bloqueados, incompatíveis ou reservados. Cadastro correto e preservação são condições para compartilhar material, não benefícios automáticos da centralização.

## Aplicação ao contexto pesquisado

A [retomada](/mro-centralizacao/retomada-contexto) reúne evidências públicas sobre as unidades paulistas e a Boa Vista, em Goiás, suas diferenças de ativos e janelas de manutenção. A leitura para MRO é:

- **(Inferência)** Avaliar a Boa Vista separadamente quanto a tempo de atendimento; não assumir desempenho logístico igual ao das unidades paulistas.
- **(Hipótese)** Materiais comuns podem permitir reservas compartilhadas, após validar especificações, substitutos e demanda simultânea.
- **(Hipótese)** Ativos específicos podem exigir proteção própria, mesmo quando outros materiais são compartilhados.
- **(Inferência)** Comparar safra e entressafra: atendimento regular satisfatório não comprova capacidade para o pico de manutenção.

Esses pontos orientam investigação. O híbrido é uma alternativa a testar, não uma recomendação automática à companhia.

## Lacunas e encaminhamento

Seriam necessários: requisições e faltas por item/unidade; criticidade e tolerância à espera; reservas de manutenção; equivalências; prazos completos e variabilidade; custos de frete e plantão; estoque utilizável e obsoleto; capacidade e preservação dos armazéns; contingências de rota. Essa base interna não está disponível nesta pesquisa.

O próximo passo seria segmentar materiais, eliminar configurações que violem restrições de serviço e segurança, dimensionar as restantes e aplicar os [critérios do benchmark](/mro-centralizacao/benchmark-praticas#criterios-de-analise). A aplicação numérica em cenário genérico pertence à [matriz multicritério](/mro-centralizacao/matriz-decisao-multicriterio), entrega distinta desta análise.

## Fontes

1. MIT CENTER FOR TRANSPORTATION & LOGISTICS. *Supply Chain Fundamentals: Key Concepts*, v. 4, 2017, seção Managing Multiple Locations. [Documento didático](https://scx-static-assets.s3.amazonaws.com/SCx%20Key%20Concept%20Documents/2-KeyConcept_Large_SV.pdf). Acesso em: 28 out. 2026.
2. BIMPIKIS, Kostas; MARKAKIS, Mihalis. *Inventory Pooling under Heavy-Tailed Demand*. Management Science, 2016. [Página dos autores e resumo](https://web.stanford.edu/~kostasb/research/pooling/). Acesso em: 28 out. 2026.
3. SCHMITT, Amanda J.; SUN, Siyuan; SNYDER, Lawrence V.; SHEN, Zuo-Jun Max. *Centralization versus decentralization: Risk pooling, risk diversification, and supply chain disruptions*. Omega, v. 52, p. 201–212, 2015. DOI: 10.1016/j.omega.2014.06.002. [Resumo do artigo](https://www.sciencedirect.com/science/article/abs/pii/S0305048314000759). Acesso em: 28 out. 2026.

As evidências empresariais usadas como contexto estão referenciadas na [retomada](/mro-centralizacao/retomada-contexto); esta página não produz novas medições da companhia.
