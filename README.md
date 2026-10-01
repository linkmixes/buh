# Buh!

Chat de IA em **um único arquivo HTML** — funciona com modelos **locais (Ollama)** e **na nuvem** (Gemini, OpenRouter, Hugging Face, Cohere…). Sem servidores, sem cadastro: tudo roda no seu navegador.

## Como usar

1. Abra o site (GitHub Pages) ou o `index.html` direto no navegador.
2. **IA local**: instale o [Ollama](https://ollama.com) e um modelo (ex.: `ollama pull qwen2.5:3b`). No Windows, permita o acesso do site ao Ollama:

   ```
   setx OLLAMA_ORIGINS "*"
   ```

   e reinicie o Ollama (ícone na bandeja → Quit → abrir de novo).
3. **IA na nuvem**: abra **Configurações → IAs**, cole a sua chave de API no provedor que quiser e ative-o. As chaves ficam salvas apenas no seu navegador (localStorage).
4. Escolha a IA no seletor — ou deixe em **Automático**, que escolhe a melhor disponível e faz *fallback* se alguma falhar.

## Recursos

- Várias conversas com **memória** (histórico completo como contexto + instruções permanentes)
- **Voz**: ditado pelo microfone e leitura das respostas em voz alta
- **Anexos**: imagens (para IAs com visão), PDFs e textos
- **Auto-reparo**: se um modelo for aposentado pela provedora, o nome é corrigido sozinho consultando a própria API; falhas temporárias são revalidadas automaticamente
- Tema claro/escuro, backup/importação de tudo em JSON
- Botão "testar" em cada IA, com relatório de status

## Privacidade

Nada é enviado para este repositório: as mensagens vão apenas para o Ollama na sua máquina ou para a API do provedor que você mesmo configurou.

## Licença

Uso livre.
