# Reconhecimento de texto com o Vision Studio

Criado um recurso no Azure Vision Studio seguindo a documentação a seguir [mslearn-ai-fundamentals (microsoftlearning.github.io)](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html)

Foi criado localmente uma pasta chamada **inputs** com as imagens com os textos que eu quero detectar, e uma pasta **output** com os resultados obtidos. Esses resultados foram detalhados passo a passo e podem ser conferidos no conteúdo desse README.

Todas as imagens foram extraídas do repositório publico a seguir: [Fotos profissionais gratuitas, imagens profissionais livres de royalties e fotos sem direitos autorais (pexels.com)](https://www.pexels.com/pt-br/)

## Configuração

1. No portal do Azure, criar um novo recurso no _Azure AI Services_ 

2. Após criado, entrar no [Vision Studio](https://portal.vision.cognitive.azure.com/?azure-portal=true)

3. Na página inicial, clique em View all resources e selecione o recurso criado como default.

![8559c978-0d2e-4009-aff8-eb5edfc93dd6](file:///C:/Users/joao.pedro/OneDrive%20-%20Capitale%20Energia/Imagens/Typedown/8559c978-0d2e-4009-aff8-eb5edfc93dd6.png)

4. Volte a página inicial do Vision Studio e vá até a aba **Optical character recognition** e em seguira **Extract text from images**.

![d133673c-fa6b-48fc-a796-6fcc1f1da84b](file:///C:/Users/joao.pedro/OneDrive%20-%20Capitale%20Energia/Imagens/Typedown/d133673c-fa6b-48fc-a796-6fcc1f1da84b.png)

5. Aqui é possível utilizar uma imagem padrão sugerida, ou anexar alguma imagem que você tenha armazenada.

## Análises e Resultados

A primeira imagem utilizada foi uma arte escrita "Take it easy", talvez pela forma e estilo que a arte foi feita, a IA não identificou a palavra IT.

![78657e9f-b055-4f63-9726-4b4c1fd8c3b2](file:///C:/Users/joao.pedro/OneDrive%20-%20Capitale%20Energia/Imagens/Typedown/78657e9f-b055-4f63-9726-4b4c1fd8c3b2.png)

A segunda imagem foi para tentar simular boletos ou formulários. Ele identificou grande parte do conteúdo das imagens, porém onde está escrito TAXES, a ferramenta trouxe cada letra fora de ordem.

![c9f97735-ec88-4158-bc7c-991d71a73a2e](file:///C:/Users/joao.pedro/OneDrive%20-%20Capitale%20Energia/Imagens/Typedown/c9f97735-ec88-4158-bc7c-991d71a73a2e.png)

A última imagem foi para tentar identificar se a ferramenta também reconhece caracteres chineses. No caso ele conseguiu reconhecer todos, porém no caracter 息 ele identificou o caracter na totalidade, porém trouxe o radical 自 como se fosse uma palavra a parte.

![900a53c7-1c24-46ed-b29b-b9fdba2ad339](file:///C:/Users/joao.pedro/OneDrive%20-%20Capitale%20Energia/Imagens/Typedown/900a53c7-1c24-46ed-b29b-b9fdba2ad339.png)

Com poucas imagens foi possível analisar que a ferramenta é muito bem treinada e pode ser usada para diferentes propósitos, porém ainda assim é sempre necessário ter uma intervenção humana para avaliar se o resultado está totalmente coerente.

Uma possibilidade seria fazer a busca textual em um grande volume de arquivos similares ou padronizados, como diversos comprovantes de pagamento para pedir reembolso, e também análise textual de faturas e notas fiscais.


