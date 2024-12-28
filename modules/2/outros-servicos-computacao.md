# Computação sem servidor

![Comparação entre computação com servidores virtuais (considerando servidores e código) e computação sem servidor (considerando apenas código)](12.png)

O termo “sem servidor” significa que o código é executado em servidores, sem que você precise provisionar ou gerenciar esses servidores. Com a computação sem servidor, você pode se concentrar na inovação de novos produtos e recursos em vez de manter servidores.

Outro benefício da computação sem servidor é a flexibilidade de dimensionar aplicações sem servidor automaticamente. A computação sem servidor pode ajustar a capacidade de aplicativos modificando as unidades de consumo, como taxa de transferência e memória. 

Um serviço da AWS para computação sem servidor é o AWS Lambda.

# AWS Lambda

O [AWS Lambda](https://aws.amazon.com/pt/lambda/) é um serviço que permite a execução de códigos sem a necessidade de provisionar ou gerenciar servidores. 

Ao usar o AWS Lambda, você paga apenas pelo tempo de computação consumido. As cobranças se aplicam ao tempo em que o código fica em execução. Você pode executar códigos para praticamente qualquer tipo de aplicativo ou serviço de back-end sem a necessidade de qualquer gerenciamento. 

Por exemplo, uma função simples do Lambda é o redimensionamento automático de imagens com o upload feito na nuvem AWS. Nesse caso, a função é acionada ao fazer upload de uma nova imagem. 

### Como o AWS Lambda funciona

![alt text](13.png)