# Definição de preços do Amazon EC2

Com o Amazon EC2, você paga apenas pelo tempo de computação que usar. O Amazon EC2 oferece diversas opções de preço para diferentes casos de uso. Por exemplo, se o seu caso de uso tolerar interrupções, você poderá economizar com as instâncias spot. Você também pode economizar assumindo um compromisso antecipadamente e bloqueando um nível mínimo de uso com instâncias reservadas.

### Sob demanda 

Isso significa que você paga somente pela duração da execução da instância. Pode ser por hora ou por segundo, dependendo do tipo de instância e do tipo do sistema operacional escolhido.

Instâncias sob demanda são ideais para cargas de trabalho irregulares de curto prazo que não podem ser interrompidas. Custos antecipados ou contratos mínimos não se aplicam. As instâncias são executadas continuamente até que sejam interrompidas, e você paga apenas pelo tempo de computação usado.

Exemplos de casos de uso para instâncias sob demanda são desenvolvimento e teste de aplicações e execução de aplicações com padrões de uso imprevisíveis. As instâncias sob demanda não são recomendadas para cargas de trabalho que duram um ano ou mais, porque essas cargas de trabalho podem ser mais econômicas usando instâncias reservadas.

### Reservadas

As instâncias reservadas são um desconto de cobrança aplicado ao uso de instâncias sob demanda na sua conta. Há dois tipos disponíveis de instância reservada:

- Standard Reserved Instances
- Instâncias reservadas conversíveis

Você pode comprar Standard Reserved Instances e instâncias reservadas conversíveis por um período de vigência de 1 ou 3 anos. Você terá maior economia de custos com a opção de três anos. 

Standard Reserved Instances: essa opção será adequada se você souber o tipo e o tamanho da instância do EC2 de que precisa para suas aplicações com estado pronto e em qual Região da AWS planeja executá-las. As instâncias reservadas exigem que você declare as seguintes qualificações:

- Tipo e tamanho da instância: Por exemplo, m5.xlarge
- Descrição da plataforma (sistema operacional): Por exemplo, Microsoft Windows Server ou Red Hat Enterprise Linux
- Tenancy: Tenancy-padrão ou dedicado

Você tem a opção de especificar uma Zona de Disponibilidade para as instâncias reservadas do EC2. Se você usar essa especificação, vai obter a reserva de capacidade do EC2. Isso garante que a quantidade desejada de instâncias do EC2 estará disponível quando você precisar delas. 

Instâncias reservadas conversíveis: se você precisar executar suas instâncias do EC2 em diferentes Zonas de Disponibilidade ou diferentes tipos de instância, as instâncias reservadas conversíveis poderão ser adequadas para você. Observação: você negocia com um desconto maior quando precisa de flexibilidade para executar suas instâncias do EC2.

No final de um período de vigência de instância reservada, você pode continuar usando a instância do Amazon EC2 sem interrupção. No entanto, são cobrados os preços de instâncias sob demanda até que um dos procedimentos a seguir seja feito:

- Terminar a instância.
- Adquirir uma nova instância reservada que corresponda aos atributos da instância (tamanho e família de instância, Região, plataforma e tenancy).

### Saving Plans

A AWS oferece Savings Plans para alguns serviços computacionais, incluindo o Amazon EC2. Os Savings Plans reduzem o custo da instância do EC2 quando você assume um compromisso de gasto por hora com uma família de instância e uma Região por um período de um ou três anos. Esse compromisso com o período de vigência resulta em uma economia de 72% em comparação com as taxas sob demanda. Qualquer uso até o compromisso é cobrado de acordo com o preço de Savings Plans com desconto (por exemplo, USD 10 por hora). Qualquer uso além do compromisso é cobrado de acordo com as taxas normais de instâncias sob demanda.



Os Savings Plans de instância do EC2 serão uma boa opção se você precisar de flexibilidade no uso do Amazon EC2 durante o período de vigência do compromisso. Você tem o benefício de reduzir o custo de execução de qualquer instância do EC2 em uma família na Região escolhida (por exemplo, uso de M5 no Norte da Virgínia), independentemente da Zona de Disponibilidade, tamanho da instância, sistema operacional ou tenancy. A economia com os Savings Plans da instância do EC2 é semelhante à economia das Standard Reserved Instances.



Ao contrário das instâncias reservadas, no entanto, você não precisa especificar antecipadamente qual tipo e tamanho da instância do EC2 (por exemplo, m5.xlarge), sistema operacional e tenancy para receber o desconto. Além disso, você não precisa se comprometer com um determinado número de instâncias do EC2 durante um período de vigência de um ou três anos. Além disso, os Savings Plans da instância do EC2 não incluem uma opção de reserva de capacidade do EC2.



Posteriormente neste curso, você conhecerá o AWS Cost Explorer, que pode ser usado para visualizar, entender e gerenciar seus custos e uso da AWS ao longo do tempo. Se você está considerando as opções dos Savings Plans, use o AWS Cost Explorer para analisar seu uso do Amazon EC2 nos últimos 7, 30 ou 60 dias. O AWS Cost Explorer também dá recomendações personalizadas para Savings Plans. Essas recomendações calculam o quanto você pode economizar mensalmente com o Amazon EC2, com base no uso anterior do Amazon EC2 e no valor do compromisso por hora em um Savings Plan de um ou três anos.


### Spot 

As instâncias spot são ideais para cargas de trabalho com horários de início e término flexíveis ou que toleram interrupções. As instâncias spot usam a capacidade de computação não utilizada do Amazon EC2 e têm até 90% de desconto em relação aos preços das instâncias sob demanda.

Suponha que você tenha um trabalho de processamento em segundo plano que pode ser iniciado e interrompido conforme for necessário (por exemplo, para uma pesquisa de cliente). Você deseja iniciar e interromper o trabalho de processamento sem afetar as operações gerais de seus negócios. Se você fizer uma solicitação spot e a capacidade do Amazon EC2 estiver disponível, a instância spot será iniciada. No entanto, se você fizer uma solicitação spot e a capacidade do Amazon EC2 estiver indisponível, a solicitação não terá sucesso até que a capacidade seja disponibilizada. A capacidade indisponível pode atrasar o início do trabalho de processamento em segundo plano.

As instâncias spot que você iniciar poderão ser interrompidas se não houver mais capacidade disponível ou se a demanda por essas instâncias aumentar. Isso pode não representar problemas para o trabalho de processamento em segundo plano. No entanto, no exemplo anterior de desenvolvimento e teste de aplicativos, é provável que você queira evitar interrupções inesperadas. Portanto, escolha um tipo de instância do EC2 diferente que seja ideal para essas tarefas.


### Host dedicadas

Os hosts dedicados são servidores físicos com capacidade de instância do Amazon EC2 totalmente dedicada ao uso do cliente. 


Você pode usar suas licenças de software por soquete, por núcleo ou por VM para manter a conformidade da licença. Você pode adquirir hosts dedicados sob demanda e reservas de hosts dedicados. De todas as opções do Amazon EC2 que foram abordadas, os hosts dedicados são os mais caros.