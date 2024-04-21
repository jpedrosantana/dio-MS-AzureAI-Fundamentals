# Analisando texto com o Azure Language Studio

Projeto 4 da Formação, com o objetivo de demonstrar um pouco do Azure Language Studio e como podemos analisar textos com essa ferramenta. Todo descritivo desse README pode ser conferido na seguinte documentação: [mslearn-ai-fundamentals (microsoftlearning.github.io)](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html)

Foi criada uma pasta input com os textos utilizados para análise.

## Configuração

1. Crie um novo resource group para o Language Service;

2. Na página Select additional features, mantenha as configurações default e prossiga com o preenchimento das informações necessárias para a criação do resource group;

3. No pricing tier, selecione o Free F0;

4. Criado o resource group, vá para a página do [[Language Studio - Microsoft Azure](https://language.cognitive.azure.com/?azure-portal=true)](https://language.cognitive.azure.com/?azure-portal=true)

5. Na tela de Select an Azure resource, preencha com seu Azure directory, subscription, resource type e resource name para ter tudo já como padrão.

6. Na página inicial, selecione a aba **Classify text** e o recurso **Analyse sentiment and mine opinions**.

7. Na tela é possível utilizar os textos de exemplo ou anexar seus próprios arquivos para a análise de sentimentos.

## Análise e resultados

Para a avaliação eu utilizei 4 reviews de restaurantes que encontrei no Google Maps, todas as reviews estão na pasta inputs.

Para cada sentença na frase, a ferramenta analisa individualmente e no final trás uma avaliação geral de todas as análise e se ela é mais positiva, negativa ou neutra.



Em cada análise a ferramenta tenta buscar as palavras chave do texto e alguns adjetivos ou complementos que definam se as palavras alvo sofrem um impacto positivo ou negativo na sentença.



Esse tipo de recurso pode ser muito útil para fazer análise de avaliações em geral, como posts em redes sociais, avaliações de filmes, produtos, lugares e serviços, sem precisar que uma pessoa faça uma análise de todos os textos escritos.
