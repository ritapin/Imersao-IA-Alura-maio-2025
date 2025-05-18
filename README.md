# Agente de IA para Criação de Posts Acadêmicos no LinkedIn

Este projeto consiste em um agente de inteligência artificial desenvolvido em Python, utilizando as ferramentas do Google Gemini (através da biblioteca `google-adk`), com o objetivo de automatizar o processo de pesquisa, resumo e criação de posts acadêmicos para a plataforma LinkedIn.

## Funcionalidades Principais:

1.  **Busca de Artigos Acadêmicos:** O `agente_buscador` utiliza a pesquisa do Google para encontrar artigos científicos, dissertações de mestrado e teses de doutorado relevantes para um tópico específico. Os resultados são filtrados para o idioma português e incluem informações sobre o tipo de documento e o link de acesso.
2.  **Resumo de Artigos:** O `agente_resumo` processa os artigos encontrados e gera resumos concisos, destacando os pontos mais relevantes de cada um. Cada resumo inclui o título, autor, data e instituição, além de uma descrição, tópicos importantes e uma conclusão. Pode utilizar a busca do Google para aprofundar informações, com devida indicação da fonte externa.
3.  **Redação de Posts para o LinkedIn:** O `agente_redator` utiliza os resumos dos artigos para criar rascunhos de posts engajadores e informativos para o LinkedIn. Os posts são escritos em um tom profissional, explicitam a principal descoberta da pesquisa, incentivam debates e incluem referências bibliográficas e hashtags relevantes.
4.  **Revisão de Qualidade:** O `agente_revisor` atua como um editor, revisando os rascunhos dos posts para garantir clareza, concisão, correção e adequação do tom para o público do LinkedIn.

## Tecnologias Utilizadas:

* Python
* Biblioteca `google-genai` (para interação com os modelos Gemini)
* Biblioteca `google-adk` (para a construção dos agentes)
* Ferramenta de Busca do Google (integrada ao Gemini)
* Bibliotecas `os`, `google.colab.userdata`, `IPython.display`, `datetime`, `textwrap`, `requests` e `warnings` para funcionalidades auxiliares.

## Como Utilizar:

1.  **Configuração da API Key:** É necessário configurar a sua chave da API do Google Gemini utilizando o `google.colab.userdata`.
2.  **Execução no Google Colab:** O código foi desenvolvido para ser executado no ambiente Google Colab.
3.  **Entrada do Tópico:** Ao executar o script, você será solicitado a inserir o tópico sobre o qual deseja criar o post.
4.  **Fluxo dos Agentes:** O sistema executa sequencialmente os quatro agentes para buscar, resumir, redigir e revisar o post.
5.  **Visualização dos Resultados:** Os resultados de cada agente são exibidos na tela utilizando a formatação Markdown.

## Próximos Passos (Sugestões):

* Implementar um sistema para salvar os posts gerados.
* Permitir a configuração de diferentes tons de escrita para o post.
* Adicionar a possibilidade de incluir imagens ou outros elementos multimídia nos posts.
* Explorar a integração com a API do LinkedIn para publicação direta.

Sinta-se à vontade para contribuir e expandir este projeto!
