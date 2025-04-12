
# 📌 Projeto: Automações para Gestores de Tráfego Pago

## 📖 Visão Geral

Este repositório contém o desenvolvimento do projeto Automações para Gestores de Tráfego Pago, cujo objetivo é automatizar a coleta, transcrição e análise de anúncios ativos na plataforma Meta (Facebook e Instagram). O projeto foi concebido para facilitar o trabalho de gestores de tráfego pago, permitindo-lhes obter insights estratégicos sobre concorrentes de maneira eficiente e automatizada.

## 🎯 Objetivo do Projeto

Desenvolver uma solução que integre a plataforma N8N com APIs externas para capturar anúncios em circulação, transcrever seu conteúdo por meio de inteligência artificial e armazenar as informações de forma estruturada. Dessa forma, os gestores de tráfego poderão analisar tendências e melhorar suas campanhas publicitárias sem a necessidade de coleta manual de dados.

## 📌 Problemática

Atualmente, a análise de anúncios da concorrência é um processo manual e ineficiente. Além disso, a Meta não oferece uma solução simples para extrair e estruturar essas informações de maneira acessível. A automação desse fluxo permitirá que profissionais de marketing economizem tempo e otimizem suas campanhas de forma baseada em dados reais.

## 🛠️ Tecnologias Utilizadas

- N8N: Plataforma low-code para automação de processos.
- APIs de terceiros: Para consulta de anúncios ativos e extração de dados.
- Inteligência Artificial: Para análise do conteúdo transcrito.
- Banco de Dados: Para armazenamento e estruturação das informações coletadas.

## 📩 Contato

Vitor Zeferino Queiroz - Desenvolvedor do projeto.  
vitor.queiroz@sou.inteli.edu.br

---

# ✅ Sprint 1 – Captura de Anúncios Ativos

## 🚀 Funcionalidade

Automatiza a coleta de vídeos de anúncios ativos na Meta com base no nome de um influenciador ou anunciante, retornando links dos vídeos, legendas, curtidas e imagens de prévia.

## 🔧 Estrutura do Workflow

1. Início manual via "Test workflow"
2. Definição de credenciais e parâmetros da API
3. Busca por contas associadas ao nome fornecido
4. Requisição de vídeos ativos
5. Formatação dos dados via JavaScript

## 📸 Exemplos

![image](https://github.com/user-attachments/assets/618cd149-e3f3-44f8-b86e-ac15f5f7cc61)

## 🛠 Conclusão

Primeira etapa do MVP finalizada com sucesso. 🚀

---

# ✅ Sprints 2/3 – Transcrição de Áudio

## 🚀 Funcionalidade

Transcreve o áudio dos anúncios coletados utilizando a API Speechflow e estrutura os dados para posterior análise.

## 🔧 Etapas do Workflow

1. Configuração e envio do áudio para a API
2. Aguardar resposta (nó Wait)
3. Recebimento da transcrição
4. Verificação condicional
5. Formatação da transcrição (texto, timestamps, metadados)

## 📸 Exemplos

![image](https://github.com/user-attachments/assets/dc2409a9-3ccf-4322-b974-1c0d8894fa44)
![image](https://github.com/user-attachments/assets/302b6cd5-97ab-4e52-aa1a-3bfe9809ef2e)

- Transcrição crua.

## 🛠 Conclusão

A integração com a Speechflow foi bem-sucedida, tornando possível extrair conteúdo falado dos anúncios.

---

# ✅ Sprint 4 – Integração com Banco de Dados (Airtable)

## 🚀 Funcionalidade

Armazena os dados coletados e processados em um banco de dados visual, acessível e estruturado no Airtable.

## 🔧 Etapas

1. Captura e transcrição dos dados
2. Criação de registros via nó "Create Record"
3. Estrutura de banco com nome, legenda, transcrição, vídeo e imagem

## 📸 Exemplo

![image](https://github.com/user-attachments/assets/c6a9bddf-85dc-463b-987e-bdb549736a67)

- Visualização do Airtable com os campos preenchidos.

## 🛠 Conclusão

Com o Airtable, os dados agora estão prontos para análises manuais e automáticas, com potencial para dashboards e IA.

---

# ✅ Sprint 5 – Validação do Fluxo e Diagnóstico de Erros

## 🚀 Funcionalidade

Testes ponta a ponta e validação do MVP, corrigindo falhas e implementando melhorias no fluxo completo.

## 🔧 Melhorias Implementadas

1. Testes completos de integração entre módulos
2. Correção de falhas de lógica e dados nulos
3. Lógicas para evitar duplicações e identificar vídeos já analisados
4. Otimização do tempo de espera da transcrição
5. Filtros para processar apenas vídeos novos

## 🧠 Novas Estratégias

- Verificações condicionais
- Garantia de sincronismo entre etapas
- Fluxo mais resiliente a falhas e atrasos

## 🛠 Conclusão

O MVP foi consolidado como uma solução funcional, confiável e pronta para as próximas etapas do projeto, incluindo análise por IA.
