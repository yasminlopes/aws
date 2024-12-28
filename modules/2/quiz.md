1. Qual tipo de instância do Amazon EC2 é adequado para aplicações de data warehousing?

- [ ] Otimizada para memória
- [x] Otimizada para armazenamento
- [ ] Uso geral
- [ ] Otimizada para computação

2. Qual tipo de instância do Amazon EC2 equilibra os recursos de computação, memória e rede?

- [ ] Otimizada para memória
- [ ] Otimizada para armazenamento
- [x] Uso geral
- [ ] Otimizada para computação

3. Qual tipo de instância do Amazon EC2 é ideal para bancos de dados de alto desempenho?

- [x] Otimizada para memória
- [ ] Otimizada para armazenamento
- [ ] Uso geral
- [ ] Otimizada para computação

4. Qual tipo de instância do Amazon EC2 é ideal para servidores web de alto desempenho?

- [ ] Otimizada para memória
- [ ] Otimizada para armazenamento
- [ ] Uso geral
- [x] Otimizada para computação

--- 

5. Qual opção de preço do Amazon EC2 oferece um desconto quando você especifica um número de instâncias do EC2 para executar um sistema operacional, família e tamanho de instância e tenancy específicos em uma Região?

- [ ] Instâncias reservadas conversíveis
- [ ] Savings Plans da instância do EC2
- [ ] Instâncias spot
- [x] Standard Reserved Instances

As Standard Reserved Instances exigem que você especifique: 

- tamanho e família de instância
- descrição da plataforma
- tenancy
- Região
  
Sua quantidade específica de instâncias do EC2 é coberta por um período de vigência de um ou três anos.

6. Qual opção de preço do Amazon EC2 oferece um desconto quando você assume um compromisso de gasto por hora com uma família de instância e uma Região por um período de vigência de um ou três anos?

- [ ] Sob demanda
- [x] Savings Plans da instância do EC2
- [ ] Instâncias spot
- [ ] Instâncias reservadas

Os Savings Plans reduzem o custo das instâncias do EC2 em troca do compromisso de um gasto por hora com uma família e uma Região, por um ou três anos. 

---

7. Qual serviço da AWS é a melhor opção para publicar mensagens para assinantes?
- [ ] Amazon Simple Queue Service (Amazon SQS)
- [ ] Amazon EC2 Auto Scaling
- [x] Amazon Simple Notification Service (Amazon SNS)
- [ ] Elastic Load Balancing

O Amazon SNS é um serviço de publicação/assinatura. Usando tópicos do Amazon SNS, um editor publica mensagens para assinantes.

As outras respostas estão incorretas porque:

- O Amazon Simple Queue Service (Amazon SQS) é um serviço de enfileiramento de mensagens. Ele não usa o modelo de assinaturas de mensagens e tópicos do Amazon SNS.
- O Amazon EC2 Auto Scaling permite que você adicione ou remova automaticamente instâncias do Amazon EC2 em resposta à alteração da demanda da aplicação.
- O Elastic Load Balancing é o serviço da AWS que distribui automaticamente o tráfego de entrada de aplicação entre vários recursos, como instâncias do Amazon EC2.