# Fundamentos de Inteligência Artificial e IA Generativa

## 1. Fundamentos de Inteligência Artificial

A **Inteligência Artificial** é o campo da ciência da computação que visa criar sistemas capazes de realizar tarefas que normalmente exigiriam inteligência humana. Essas tarefas incluem raciocínio, aprendizado, percepção, tomada de decisão e compreensão de linguagem.

### Tipos de IA

- **IA Fraca:** Projetada para uma tarefa específica. Ex: Assistentes virtuais.
- **IA Forte:** Capaz de realizar qualquer tarefa cognitiva humana. Ainda em estágio teórico.

### Subcampos da IA

- Visão Computacional
- Processamento de Linguagem Natural (PLN)
- Robótica
- Aprendizado de Máquina (Machine Learning)
- Sistemas Especialistas

---

## 2. Fundamentos de IA Generativa

**IA Generativa** refere-se a sistemas de IA que são capazes de gerar novos dados que se assemelham a dados de entrada usados para treiná-los. Exemplos: gerar texto, imagens, música, código ou até moléculas químicas.

### Modelos Populares

- **GPT**
- **DALL·E**

### Aplicações

- Criação de conteúdo automatizado
- Assistência em programação
- Geração de imagens e áudio
- Simulação de dados para testes

---

## 3. Fundamentos de Aprendizado de Máquina

O **Aprendizado de Máquina** é um subconjunto da IA que permite que sistemas aprendam a partir de dados sem serem explicitamente programados.

### Tipos de Aprendizado

- **Supervisionado:** O modelo aprende com dados rotulados.
- **Não supervisionado:** O modelo busca padrões em dados não rotulados.
- **Aprendizado por Reforço:** Um agente aprende com base em recompensas/punições em um ambiente.

### Principais Algoritmos

- Regressão Linear e Logística
- Árvores de Decisão
- Máquinas de Vetores de Suporte (SVM)
- Redes Neurais Artificiais
- K-means (para clustering)

---

## 4. Conceitos de Processamento de Linguagem Natural

O **PLN** é o campo da IA que lida com a interação entre computadores e a linguagem humana.

### Tarefas de PLN

- **Tokenização:** Dividir texto em palavras ou frases.
- **Lematização:** Reduzir palavras à sua forma base.
- **Análise Sintática:** Compreender a estrutura gramatical.
- **Reconhecimento de Entidades Nomeadas (NER):** Identificar nomes de pessoas, locais, etc.
- **Análise de Sentimentos:** Identificar a opinião expressa no texto.

### Técnicas e Ferramentas

- Bag of Words
- TF-IDF
- Embeddings (ex: Word2Vec, GloVe)
- Transformers (ex: BERT, GPT)

---

## 5. Análise de Sentimentos com Azure AI - Language Studio

O **Language Studio** do Azure é uma interface gráfica que permite utilizar os serviços de linguagem da Microsoft com pouca ou nenhuma codificação.

### Passos para Análise de Sentimentos no Language Studio

- **Acesse o Language Studio**
   - URL: [https://language.azure.com](https://language.azure.com)

- **Escolha a Análise de Sentimentos**
   - Serviço que determina a polaridade (positivo, negativo, neutro) de textos.

- **Insira o Texto**
   - Pode inserir textos em diferentes idiomas.

- **Interprete os Resultados**
   - A resposta inclui:
     - **Pontuações por sentimento** 
     - **Frases-chave extraídas**
     - **Sentimento por sentença**

- **Exportar ou Integrar**
   - Os resultados podem ser exportados como JSON ou integrados via API REST.

### Exemplo de Resultado (JSON simplificado)

```json
{
  "sentiment": "positive",
  "confidenceScores": {
    "positive": 0.91,
    "neutral": 0.08,
    "negative": 0.01
  },
  "sentences": [
    {
      "text": "Adorei o atendimento e voltarei mais vezes!",
      "sentiment": "positive"
    }
  ]
}
