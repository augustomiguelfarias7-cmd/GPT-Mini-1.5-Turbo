===============================
GPT-Mini 1.5 Turbo - Guia de Uso
===============================

Descrição do modelo:
-------------------
O GPT-Mini 1.5 Turbo é um modelo de linguagem baseado no GPT-Mini normal, com funcionalidades avançadas de multimodalidade.
Ele consegue:
- Gerar texto em português brasileiro e em outros idiomas.
- Compreender e analisar imagens (visão computacional).
- Processar e transcrever áudio.
- Gerar imagens a partir de prompts de texto (via modelo integrado de geração de imagens).

Funcionalidades principais:
---------------------------
1. Texto:
   - Geração de texto coerente e contextual.
   - Compatível com prompts curtos e longos.

2. Imagem:
   - Recebe imagens como entrada e gera embeddings para análise.
   - Permite integração com prompts de imagens para gerar descrições ou respostas multimodais.

3. Áudio:
   - Transcrição de arquivos de áudio.
   - Conexão com embeddings de áudio para multimodalidade.

4. Geração de Imagens:
   - Aceita prompts de texto e gera imagens correspondentes usando o modelo DALL·E integrado.
   - Retorna imagens em formato RGB padrão.

Comparação com GPT-Mini normal:
-------------------------------
- GPT-Mini 1.5 Turbo mantém a base do GPT-Mini normal.
- Adiciona suporte multimodal (imagem e áudio) e geração de imagens.
- Mantém compatibilidade com pipelines Transformers.
- Pode ser usado para tarefas de NLP, visão e áudio no mesmo modelo.

Como usar:
----------
1. Carregar o modelo:
   ```python
   from transformers import AutoModelForCausalLM, AutoTokenizer

   tokenizer = AutoTokenizer.from_pretrained("./GPT-Mini-1.5-Turbo")
   model = AutoModelForCausalLM.from_pretrained("./GPT-Mini-1.5-Turbo")
  
