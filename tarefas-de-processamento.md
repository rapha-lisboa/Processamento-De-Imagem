# Tarefas de processamento de imagem

## I Introdução

Neste documento iremos abordar sobre duas tarefas de processamento de imagem. Processamento de imagem é uma etapa de visão computacional, que no caso é uma forma de utilizar o aprendizado de máquina para o auxilio em diversas tarefas como por exemplo a identificação de alimentos inadequados ao consumo em uma esteira de produção, identificação de talhões em imagens de satélite, entre outros.

## II Discussão

Existem diversas formas que permitem com que um computador seja capaz de identificar de imagens, vamos abordar nessa sessão algumas delas, mas antes de explica-las primeiro é preciso exclarecer o que é uma imagem a níveis de entendimento de um computador. Basicamente uma imagem é uma matriz de 2 dimensões em que cada elemento da matriz é representado por um píxel, que não é nada mais nada menos que um ponto na tela do computador na qual emite uma luz, variando a cor, tom e intensidade luminosa. Para que ele tome uma alta possibilidade de representações ele pode ser tratado por 1 ou mais camadas, comumente quando ele é representado por 1 camada estamos falando de uma mesma cor que varia apenas a tonalidade indo do mais escuro possível, outra forma muito comum utilizada é o famoso RGB em que o píxel é representado por 3 camadas: uma para o vermelho, uma para o verde e uma para o azul.


### 2.1 Classificação de imagem

Tendo como uma imagem é interpretada por um computador em consideração, a classificação de imagens consiste em um processo de decisão no qual o grupo de pixels é definido como pertencente a uma determinada classe na qual uma imagem pode possuir uma ou várias classes, desta forma a máquina durante o aprendizado é exposta à várias imagens com labels indicando a classe que pertence, no fim o intuito é que o modelo responda uma distribuição da probabilidade do item que está sendo analisado ser ded cada uma das classes, que idealmente o modelo convirja com que em todos os casos ele responda 100% para a classe correta.
Um exemplo que pode ser citado é a classificação de 0 a 9 de números manuscritos, dados pelo dataset MNIST, nesse exercício o intúito é que com uma imagem a máquina seja capaz de identificar qual número está sendo analisado.

#### 2.1.1 Aplicação de mercado

Uma das aplicações de mercado que podemos fazer com essa tarefa é por exemplo a identificação de imperfeições em embalagens de uma linha de produção. Suponhamos o cenário em que em uma linha de produção tenham caixas perfeitamente embaladas, caixas amassadas que devem ser descartadas e caixas vazias que devem voltar para o inicio da produção sem serem descartadas. Para essa tomada de decisão, podemos colocar uma câmera posicionada em um lugar estratégico que com visão computacional identifique à qual classe as caixas analisadas pertencem.

#### 2.1.2 Produtos comerciais relacionados

Um produto que também aproveita essa tarefa para sua utilização são as câmeras sensoriais que se encontram ao redor dos carros da Tesla que apresentam a direção automática. Os carros utilizam dessa tecnologia para a identificação de demais veículos, motocicletas, pedestres, entre outros obstáculos que podem estar em volta do carro, dessa forma a direção autônoma utiliza isso para decidir o movimento que irá fazer, evitando assim acidentes.

### 2.2 Segmentação Semântica

Diferente da tarefa de classificação citada no tópico 2.1, onde uma classe pré-definida é identificada como pertencente à imagem ou não a tarefa de segmentação semântica vai buscar compreender a imagem completa e dessa forma dizer o que é cada conjunto de pixeis que formam um elemento único, desta forma geralmente os outputs são indicados por meio de contornos coloridos, imagens de calor, posicionamentos entre outros.

#### 2.2.1 Aplicação de mercado

Muitos procedimentos clínicos comuns, como tomografias computadorizadas (TCs), raios-X e ressonância magnética, dependem da análise de imagem. Embora normalmente essa tarefa tenha ficado a cargo de profissionais da área médica no passado, atualmente os modelos de segmentação de imagens médicas estão obtendo resultados semelhantes. Analisando a imagem e traçando limites exatos em torno dos vários objetos nela contidos, a IA equipada com segmentação semântica pode ajudar a detectar anomalias e até mesmo sugerir possíveis diagnósticos.

#### 2.2.2 Produtos comerciais relacionados

Através de técnicas como a segmentação semântica, lugares como o Amazon GO, um mercado totalmente autônomo em que os clientes apenas pegam os produtos e o valor é automaticamente debitado da conta atrelada ao login da amazon são possíveis, já que podemos utilizar a visão computacional como o controle de estoque, identificando quando um produto some de vista e assim ele pode ser atrelado à um ID cadastrado para saber o preço do produto que sumiu.

## III Conclusão

Dessa forma concluimos que muitos problemas que existem há anos, podem apresentar suas soluções vinculadas à visão computacional, visto que o intuito é que com o passar dos anos o poder computacional se aproxime cada vez mais do poder que um cérebro humano possui. O cérebro humano é altamente eficiente na identificação de padrões por meio da visão e é se inspirando nele que as pesquisas avançam e tomam um rumo cada vez mais evoluido.