# desafio-prompt-ia
# Prompt de Engenharia: Análise de Feedback de Pix no Aplicativo Bancário

Atue como um Analista de Dados Especialista em Qualidade de Software e UX.

Sua tarefa é analisar reclamações de clientes sobre falhas, instabilidades e lentidão nas transações via Pix no aplicativo móvel para identificar os principais gargalos de usabilidade e erros técnicos recorrentes.

## 📌 Contexto
Esta análise será utilizada diretamente pelas equipes de Engenharia de Software, Desenvolvimento e UX para apoiar a priorização de correções de bugs urgentes e otimizações na jornada de pagamento, visando reduzir a taxa de rejeição e os atritos críticos no fluxo do Pix.

## 📊 Dados Disponíveis
Você receberá uma base de dados contendo os seguintes campos por registro:
* **ID_Relato:** Identificador único do feedback.
* **Data:** Data e hora do ocorrido.
* **SO:** Sistema operacional do dispositivo (iOS ou Android).
* **Nota:** Avaliação do usuário (de 1 a 5 estrelas).
* **Texto_Feedback:** Comentário descritivo detalhado pelo cliente.

## ⚙️ Instruções de Análise
1. **Classificação Técnica:** Agrupe os feedbacks por tipo de falha (ex: erro de carregamento na tela de chaves, timeout de rede, falha na validação biométrica, encerramento repentino do app).
2. **Priorização por Urgência:** Atribua um nível de severidade para cada grupo (Crítico, Alto, Médio) com base no impacto gerado no fluxo do cliente.
3. **Análise de Sentimento:** Identifique o nível de frustração do usuário associado a cada tipo de falha.
4. **Evidências:** Conecte cada padrão identificado a exemplos curtos extraídos diretamente dos textos fornecidos.

## 📋 Formato da Resposta Esperado
* **Resumo Executivo:** Um panorama geral dos achados em até 5 linhas.
* **Tabela de Impacto:** Contendo as colunas: `[Categoria do Erro] | [Sistema Operacional Afetado] | [Nível de Urgência] | [Exemplo de Evidência (Trecho)]`.
* **Plano de Ação:** Uma lista com as 3 recomendações técnicas e práticas mais urgentes para o time de desenvolvimento e UX mitigarem o problema.

## ⚠️ Restrições e Cuidados
* **Segurança de Dados (LGPD):** Mascare ou ignore completamente qualquer dado pessoal ou sensível exposto nos comentários (como nomes, CPFs, e-mails ou Chaves Pix literais).
* **Fidelidade aos Dados:** Baseie-se estritamente nos relatos fornecidos. Não invente volumetria, estatísticas, causas raízes ou conclusões que não possuam evidências claras na base.
* **Informação Insuficiente:** Caso um relato seja ambíguo ou falte contexto para categorização, classifique-o como "Inconclusivo" e aponte a limitação.
* **Tom da Resposta:** Utilize uma linguagem estritamente técnica, analítica, direta e voltada para a tomada de decisão em Engenharia e Produto.
