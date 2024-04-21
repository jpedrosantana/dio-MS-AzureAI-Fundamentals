# Reconhecimento de texto com o Vision Studio

Criado um recurso no Azure Vision Studio seguindo a documentação a seguir [mslearn-ai-fundamentals (microsoftlearning.github.io)](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html)

Foi criado localmente uma pasta chamada **inputs** com as imagens com os textos que eu quero detectar, e uma pasta **output** com os resultados obtidos. Esses resultados foram detalhados passo a passo e podem ser conferidos no conteúdo desse README.

Todas as imagens foram extraídas do repositório publico a seguir: [Fotos profissionais gratuitas, imagens profissionais livres de royalties e fotos sem direitos autorais (pexels.com)](https://www.pexels.com/pt-br/)

## Configuração

1. No portal do Azure, criar um novo recurso no _Azure AI Services_ 

2. Após criado, entrar no [Vision Studio](https://portal.vision.cognitive.azure.com/?azure-portal=true)

3. Na página inicial, clique em View all resources e selecione o recurso criado como default.
   
   ![](/03_Reconhecimento_Facial_e_transformacoes_de_imagens_em_Dados_no_Azure_ML/inputs/default-resource.png?raw=True "Default resource")

4. Volte a página inicial do Vision Studio e vá até a aba **Optical character recognition** e em seguira **Extract text from images**.

5. E então será possível utilizar uma imagem padrão sugerida, ou anexar alguma imagem que você tenha armazenada.

## Análises e Resultados

A primeira imagem utilizada foi uma arte escrita "Take it easy", talvez pela forma e estilo que a arte foi feita, a IA não identificou a palavra IT.

![](/03_Reconhecimento_Facial_e_transformacoes_de_imagens_em_Dados_no_Azure_ML/outputs/output1.png?raw=True "output1")

A segunda imagem foi para tentar simular boletos ou formulários. Ele identificou grande parte do conteúdo das imagens, porém onde está escrito TAXES, a ferramenta trouxe cada letra fora de ordem.

![](/03_Reconhecimento_Facial_e_transformacoes_de_imagens_em_Dados_no_Azure_ML/outputs/output2.png?raw=True "output2")

A última imagem foi para tentar identificar se a ferramenta também reconhece caracteres chineses. No caso ele conseguiu reconhecer todos, porém no caracter 息 ele identificou o caracter na totalidade, porém trouxe o radical 自 como se fosse uma palavra a parte.

![](/03_Reconhecimento_Facial_e_transformacoes_de_imagens_em_Dados_no_Azure_ML/outputs/output3.png?raw=True "output3")

Com poucas imagens foi possível analisar que a ferramenta é muito bem treinada e pode ser usada para diferentes propósitos, porém ainda assim é sempre necessário ter uma intervenção humana para avaliar se o resultado está totalmente coerente.

Uma possibilidade seria fazer a busca textual em um grande volume de arquivos similares ou padronizados, como diversos comprovantes de pagamento para pedir reembolso, e também análise textual de faturas e notas fiscais.


