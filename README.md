# 🏦 IA-FEEDBACK-CLIENTES-BANCARIOS

## Desafio Criativo — Extraindo Insights do Feedback de Clientes Bancários

Projeto desenvolvido como parte do **Bootcamp Banco Bradesco — GenAI, Dados & Cyber**, da **Digital Innovation One (DIO) em parceria com o Banco Bradesco**.

O desafio propõe o desenvolvimento de um prompt estruturado para utilizar Inteligência Artificial na análise de feedbacks de clientes bancários, transformando manifestações dos clientes em informações que possam apoiar a identificação de padrões, problemas, riscos e oportunidades de melhoria.

---

## 🎯 Objetivo

Transformar a **voz do cliente em inteligência operacional**, utilizando IA para organizar e interpretar feedbacks bancários com base em evidências, apoiando a priorização de melhorias, riscos e oportunidades na operação bancária.

A proposta é utilizar a IA como apoio à análise e à tomada de decisão humana, sem substituir a avaliação das áreas responsáveis.

---

## 💡 Problema

Feedbacks de clientes podem conter:

- reclamações;
- elogios;
- dificuldades;
- sugestões;
- percepções;
- relatos relacionados a produtos, serviços e canais de atendimento.

Quando analisados de forma estruturada, esses registros podem revelar padrões da experiência do cliente, recorrências, oportunidades de melhoria e possíveis sinais que mereçam monitoramento ou investigação.

O desafio consiste em construir um prompt capaz de orientar a IA nessa análise de maneira estruturada, contextualizada e responsável.

---

## 🧠 Abordagem

O prompt foi desenvolvido considerando os principais elementos propostos pelo desafio:

1. **Intenção da análise**
2. **Contexto do problema**
3. **Dados de entrada**
4. **Critérios de análise**
5. **Formato da resposta**
6. **Restrições e governança**

A análise foi estruturada para considerar informações como:

- Data;
- Canal;
- Produto/Serviço;
- Texto do Feedback;
- Nota de Satisfação.

Outros campos somente devem ser utilizados quando efetivamente fornecidos nos dados de entrada.

---

## 🔎 O que a IA deve analisar

O prompt orienta a IA a:

- classificar temas e sentimentos;
- identificar produtos, serviços e canais relacionados aos feedbacks;
- diferenciar reclamações, elogios, dificuldades, sugestões e relatos;
- identificar padrões e recorrências;
- observar possíveis concentrações de manifestações;
- considerar a dimensão temporal quando houver datas;
- apresentar evidências para os insights identificados;
- reconhecer possíveis sinais operacionais ou de segurança;
- propor ações relacionadas aos insights;
- indicar as limitações da análise.

---

## ⚖️ Fato, padrão, sinal, hipótese e conclusão

Um dos princípios centrais do prompt é evitar que a IA transforme automaticamente uma manifestação em uma conclusão.

A análise diferencia:

| Categoria | Significado |
|---|---|
| **Fato** | Informação diretamente observada nos dados |
| **Padrão** | Recorrência ou comportamento observado na amostra |
| **Sinal** | Evidência que merece atenção ou monitoramento |
| **Hipótese** | Possível interpretação que ainda precisa ser validada |
| **Conclusão** | Interpretação sustentada por evidências suficientes |

Essa diferenciação busca reduzir interpretações indevidas e preservar a qualidade da análise.

---

## 🛡️ Governança e segurança

O prompt estabelece restrições para evitar conclusões não sustentadas pelos dados.

Entre as principais regras:

- utilizar somente os dados fornecidos;
- não inventar números, percentuais, causas ou conclusões;
- não preencher informações ausentes por inferência;
- não confundir correlação com causalidade;
- não tratar um feedback negativo isolado como prova de falha sistêmica;
- não confirmar fraude ou incidente de segurança sem evidências suficientes;
- não expor dados pessoais, financeiros ou sensíveis;
- informar limitações quando os dados forem insuficientes;
- manter a decisão final sob responsabilidade humana.

Também não são assumidas arquiteturas ou tecnologias específicas, como Edge Computing, Cloud ou IoT, quando essas informações não estiverem presentes nos dados fornecidos.

---

## 📊 Priorização

A priorização foi estruturada para evitar classificações baseadas apenas na percepção de gravidade de um tema.

Quando disponíveis, são considerados:

- evidência observável;
- recorrência;
- concentração de manifestações;
- relevância para a experiência do cliente;
- possível impacto operacional observável;
- necessidade aparente de atenção.


As categorias de prioridade utilizadas são:

- **Alta**
- **Média**
- **Baixa**
- **Não determinada**

Quando houver um sinal que exija investigação, mas os dados não forem suficientes para estabelecer uma prioridade confiável, a análise poderá indicar **"Necessita investigação"**, acompanhada da justificativa correspondente.

---

## 🧪 Validação do Prompt

O prompt passou por um processo de validação utilizando bases fictícias de feedbacks bancários.

### Teste 1

Foi utilizada uma amostra inicial para verificar se a IA conseguia:

- identificar recorrências;
- reconhecer sinais de segurança;
- organizar os feedbacks;
- apresentar recomendações;
- respeitar as limitações dos dados.

**Resultado:** funcionamento adequado, com identificação de uma fragilidade na definição das prioridades.

### Teste 2

Foi utilizada uma segunda amostra contendo situações mais ambíguas e contraditórias.

O teste confirmou que a principal fragilidade permanecia relacionada à possibilidade de atribuição subjetiva de prioridade.

### Refinamento

A regra de priorização foi aprimorada para exigir evidências suficientes e permitir a classificação **"Não determinada"** ou **"Necessita investigação"** quando os dados não forem suficientes.

### Teste 3 — Validação Final

Uma terceira base, construída para testar situações recorrentes, contraditórias, vagas e relacionadas à segurança, foi utilizada para validar o refinamento.

O prompt demonstrou capacidade de:

- reconhecer recorrências sem afirmar causalidade;
- diferenciar sinais de incidentes confirmados;
- tratar informações ausentes sem inventá-las;
- preservar experiências positivas e negativas;
- lidar com feedbacks vagos;
- evitar atribuição automática de alta prioridade;
- indicar quando uma prioridade não pode ser determinada de forma confiável.

**Resultado: Prompt validado.**

---

## 📁 Arquivo principal

O prompt desenvolvido está disponível em:

👉 [Prompt — Da Voz do Cliente à Inteligência Operacional](prompt-voz-cliente-inteligencia-operacional.md)


## 📌 Resultado

O resultado deste desafio é um **prompt estruturado e validado para análise de feedbacks de clientes bancários**, com foco em:

**Voz do Cliente → Dados → Evidências → Insights → Priorização → Apoio à Decisão**

A proposta busca demonstrar como a Inteligência Artificial pode apoiar a transformação de dados qualitativos em informações estruturadas, mantendo critérios de análise, transparência, segurança e governança.

---

## ⚠️ Aviso

Este projeto possui finalidade **educacional** e utiliza exemplos fictícios para validação do prompt.

O resultado produzido pela IA não deve ser utilizado como decisão operacional definitiva, diagnóstico de incidentes, confirmação de fraude ou avaliação individual de clientes.

---

## 👩‍💻 Autora

**Barbara Nascimento de Freitas**

Projeto desenvolvido no **Bootcamp Banco Bradesco — GenAI, Dados & Cyber | DIO**.

---


