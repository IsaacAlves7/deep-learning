# 🕳️ DL - Deep Learning
<a href=""><img src="https://img.shields.io/badge/Google_Colab-DL-tomato?style=flat&logo=GoogleColab&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Google_Colab-DL-tomato?style=flat&logo=GoogleColab&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Google_Colab-DL-4285F4?style=flat&logo=GoogleColab&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Google_Colab-DL-4285F4?style=flat&logo=GoogleColab&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Jupyter-DL-orange?style=flat&logo=Jupyter&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/R-DL-FEC111?style=flat&logo=R&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Tensorflow-DL-FEC111?style=flat&logo=Tensorflow&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Keras-DL-red?style=flat&logo=Keras&logoColor=white"></a>

<img src="https://github.com/user-attachments/assets/5d79cec0-d4be-4f77-9256-8eeabc463014" height="77" align="right">

O **Deep Learning** (Aprendizagem profunda) é uma subárea do Machine Learning que utiliza <a href="">redes neurais artificiais profundas</a> para modelar e resolver problemas complexos. É chamado de "profundo" (deep) porque as redes neurais usadas possuem várias camadas ocultas, permitindo que o modelo aprenda representações em diferentes níveis de abstração. 

É um subconjunto especializado de ML que utiliza redes neurais artificiais com múltiplas camadas para modelar padrões complexos em dados. Redes neurais são modelos computacionais inspirados na rede de neurônios do cérebro humano. Redes neurais profundas podem descobrir automaticamente representações necessárias para detecção futura. Casos de uso incluem reconhecimento de imagem e fala, PLN e veículos autônomos.

A aprendizagem profunda, do inglês Deep Learning (também conhecida como aprendizado estruturado profundo, aprendizado hierárquico ou aprendizado de máquina profundo) é um ramo de aprendizado de máquina (Machine Learning) baseado em um conjunto de algoritmos que tentam modelar abstrações de alto nível de dados usando um grafo profundo com várias camadas de processamento, compostas de várias transformações lineares e não lineares.

A aprendizagem profunda é parte de uma família mais abrangente de métodos de aprendizado de máquina baseados na aprendizagem de representações de dados. 

Uma observação (por exemplo, uma imagem), pode ser representada de várias maneiras, tais como um vetor de valores de intensidade por pixel, ou de uma forma mais abstrata como um conjunto de arestas, regiões com um formato particular, etc. Algumas representações são melhores do que outras para simplificar a tarefa de aprendizagem (por exemplo, reconhecimento facial ou reconhecimento de expressões faciais). 

Uma das promessas da aprendizagem profunda é a substituição de características feitas manualmente por algoritmos eficientes para a aprendizagem de características supervisionada ou semissupervisionada e extração hierárquica de características.

A pesquisa nesta área tenta fazer representações melhores e criar modelos para aprender essas representações a partir de dados não rotulados em grande escala. Algumas das representações são inspiradas pelos avanços da neurociência e são vagamente baseadas na interpretação do processamento de informações e padrões de comunicação em um sistema nervoso, tais como codificação neural que tenta definir uma relação entre vários estímulos e as respostas neuronais associados no cérebro. 

Esse mindmap reúne praticamente todo o ciclo de vida de um modelo, desde a coleta de dados até o deployment em produção, e ele mistura conceitos técnicos, matemáticos e até processos de engenharia de software. É como se fosse uma espinha dorsal que mostra o que realmente sustenta uma solução de deep learning moderna.

<img src="https://github.com/user-attachments/assets/d7aa99bd-447b-499f-82b9-c2b86f99a053" align="right">

Tudo sempre começa com dados, e é por isso que a etapa de **Data Collection and Preparation** é tão crucial. Nela você lida com a origem dos dados, com a qualidade deles e com a forma como eles chegam até você. É aqui que entram os tipos de dados, os formatos (imagens, texto, áudio, tabelas), os métodos de amostragem e a validação para garantir que nada está contaminado ou enviesado. Ao mesmo tempo, a parte de data governance cria regras para garantir que os dados têm procedência, segurança e autorização de uso. A transformação dos dados, como normalização, padronização ou categorizações, prepara o terreno para o learning acontecer mais à frente.

Depois disso, há o grande domínio de **Feature Engineering**, que é o processo de transformar dados brutos em representações mais úteis e informativas. É onde você cria atributos polinomiais, lida com valores ausentes, reduz dimensionalidade, faz encoding de categorias e extrai padrões ou características relevantes. Em modelos profundos, especialmente em imagens e texto, a feature engineering clássica diminui, mas nunca desaparece totalmente; mesmo em CNNs e transformers, você ainda prepara dados, escolhe forma de tokenização e define como os dados entram nas camadas.

A próxima fase natural é Model Selection, onde você escolhe qual arquitetura ou abordagem funciona melhor para o problema. Nesse processo, usa validação cruzada, métodos estatísticos, regularização e testes de hipótese para entender o comportamento do modelo. Aqui também entram os critérios de seleção, como variância, viés, overfitting ou underfitting, e as métricas que ajudam a comparar modelos diferentes. Esse processo sempre envolve medir, comparar e refinar.

Curiosamente o diagrama colocou também Architecture Design como um bloco — normalmente isso está dentro da seleção de modelos, mas vale entender a lógica: a arquitetura é o desenho da rede, a forma como as camadas se conectam. Apesar do mapa mostrar softwares de design arquitetural como SketchUp e AutoCAD, isso parece ter sido um erro comum nesses diagramas gerados automaticamente, porque o real sentido aqui é projetar a topologia da rede: número de camadas, tipos de camadas, conexões, profundidade, largura e formato de entrada. Essa é a parte de criar o “esqueleto” do modelo.

Então chegamos na Initialization, que é como as variáveis internas do modelo são inicialmente configuradas. Não parece importante à primeira vista, mas é absolutamente crítico. Inicialização ruim causa gradientes explosivos, gradientes desaparecendo ou um começo enviesado. Técnicas como Xavier initialization ou He initialization existem justamente para garantir que os primeiros passos do aprendizado não causem instabilidade.

Forward Propagation é o processo onde a informação literalmente viaja pela rede em direção ao output. Cada camada transforma a entrada, multiplica pesos, aplica funções de ativação e passa adiante o resultado. É a etapa do cálculo da predição bruta, onde você vê o que a rede acha que deve ser a saída. É pura matemática aplicada: matrizes, multiplicações, ativações e fluxos de dados.

A partir daí, entramos em Loss Function Calculation, que é quando comparamos a predição com a verdade. É o coração do aprendizado supervisionado. A loss diz “o quão errado você está”. Funções como cross-entropy, MSE, hinge, MAE e KL-divergence moldam o tipo de aprendizagem. Diferentes problemas exigem diferentes losses — classificação precisa de losses diferentes da regressão.

Quando o modelo sabe o quanto errou, chega a hora do Backpropagation, que calcula como ajustar os pesos ao longo da rede. Isso envolve gradientes, derivações, cadeia de cálculo, e também problemas como vanishing e exploding gradients. Essa etapa é como se fosse a “engenharia” interna do aprendizado, onde você encontra quais ajustes matemáticos devem ser feitos em cada neurônio.

Esses ajustes são aplicados na fase de **Parameter Update** aqui entram otimizações básicas e avançadas: SGD, momentum, Adam, RMSProp, AdaGrad, todos servindo para mover os pesos na direção correta. É a parte do ciclo onde o conhecimento realmente se acumula. Transfer learning, meta-learning e few-shot learning são variações modernas desse processo, que tornam o aprendizado mais eficiente ou adaptável.

Depois disso, entramos em **Gradient Descent** como grande conceito que permeia quase tudo. É a lógica contínua de minimizar a perda movendo-se gradualmente em um espaço de parâmetros. Existem variações como batch, mini-batch, estocástico, e elas influenciam estabilidade, velocidade e generalização.

**Regularization** é onde você impede que o modelo decore os dados. L1, L2, dropout, early stopping, normalização, penalidades de complexidade e data augmentation existindo justamente para tornar a rede robusta. Sem regularização, qualquer modelo profundo grande demais simplesmente memoriza os dados e fracassa em generalização.

**Hyperparameter Tuning** é o processo doloroso, demorado e indispensável de testar configurações possíveis. Coisas como taxa de aprendizado, número de camadas, tamanho do batch, dropout e muitas outras precisam ser ajustadas. Métodos como random search, grid search ou até algoritmos bayesianos ajudam a encontrar combinações melhores sem testar tudo.

Chegando ao fim do ciclo, **Model Evaluation** é o momento em que você realmente mensura performance. Aqui você analisa acurácia, erros, bias/fairness, explicabilidade e estabilidade. É onde você descobre se seu modelo está realmente aprendendo ou só fingindo, e onde você testa robustez, generalização e possíveis falhas estruturais.

Por fim, **Deployment** é a última etapa, onde tudo vira algo real. É quando o modelo sai do notebook e entra em produção: integrações, pipelines, versionamento, rollback, observabilidade, escalabilidade e infraestrutura automatizada. Aqui se trata de gerenciar modelos como sistemas vivos que precisam de manutenção, monitoramento, re-treinamento e cuidado contínuo.

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/b8ffdc54-4805-469e-b7b0-c72d35cbb0f4" height="777"></td>
    <td><img src="https://github.com/user-attachments/assets/cf526c93-fefc-4317-849d-67539f87fb73" height="777"></td>
    <td><img src="https://github.com/user-attachments/assets/3ee455a7-9c98-4dc5-b952-916ca866f08f" height="777"></td>
  </tr>
</table>

A diferença entre Machine Learning e Deep Learning:

<div align="center"><img src="https://github.com/user-attachments/assets/3abe1ef5-1e3e-4c25-be39-55f63ebc92e3"></div>

Várias arquiteturas de aprendizagem profunda, tais como:

- <a href="">Redes neurais profundas (RNPs)</a>: são um tipo de modelo de aprendizado de máquina inspirado na estrutura e funcionamento do cérebro humano.
  
- <a href="">Redes neurais profundas convolucionais (CNNs)</a>: RNCs são um tipo de rede neural profunda especialmente projetada para processar dados com estrutura espacial ou temporal, como imagens, vídeos e sinais de áudio.

- <a href="">Redes de crenças profundas (DBNs)</a>: RCPs são um tipo de modelo de aprendizado de máquina que combina elementos de redes neurais e modelos gráficos probabilísticos.

- <a href="">Redes neurais recorrentes (RNNs)</a>: RNRs são um tipo de modelo de aprendizado de máquina que é especialmente projetado para processar dados sequenciais, como texto, fala, séries temporais, etc.

Essas têm sido aplicadas em áreas como visão computacional, reconhecimento automático de fala, processamento de linguagem natural, reconhecimento de áudio e bioinformática, onde elas têm se mostrado capazes de produzir resultados do estado-da-arte em várias tarefas.

> Aprendizagem profunda foi caracterizada como a expressão na moda, ou uma recaracterização das redes neurais.

<img src="https://upload.wikimedia.org/wikipedia/commons/a/ae/Keras_logo.svg" height="77" align="right">

O **Keras** é uma API de aprendizado profundo projetada para seres humanos, não Máquinas. Keras se concentra na velocidade de depuração, elegância do código e concisão, capacidade de manutenção e capacidade de implantação. Quando você escolhe Keras, sua base de código é menor, mais legível, mais fácil de iterar em. Com sua abordagem multi-back-end (multi-framework), o Keras oferece a liberdade de trabalhar com JAX, TensorFlow e PyTorch. Crie modelos que podem se mover perfeitamente entre essas estruturas e aproveitar os pontos fortes de cada ecossistema.

<img width="1143" height="2048" alt="672681474_4547678532119655_6574815170104942009_n" src="https://github.com/user-attachments/assets/69726d22-0fb5-4550-bcd9-c8b66f6b9bf9" />

<img width="1080" height="1350" alt="670509759_1375143264633284_1081615128915418390_n" src="https://github.com/user-attachments/assets/04813e5f-d07d-43ff-938e-9e07a6ed5d58" />

![622402951_1464513672346645_4888751637558602075_n](https://github.com/user-attachments/assets/64af0d99-70dc-4b97-97c4-4a573cf558b0)

![588332797_868753202341499_6161281450660469596_n](https://github.com/user-attachments/assets/2687d748-81a6-46d0-bfb9-f371e751c393)

![infografico](https://github.com/user-attachments/assets/f5af48d7-ee43-4d79-85eb-fa1e998593de)

## [DL] Neural Network Feed-forward
<img height="77" align="right" src="https://github.com/user-attachments/assets/735eeb46-93a2-4539-b4a8-b4646fa7eba9" />

Uma **Neural Network Feed-forward** (Rede Neural de Alimentação Direta) é o modelo mais fundamental dentro do campo do *Deep Learning* e do *Machine Learning* em geral. Ela é chamada assim porque os sinais, ou seja, os dados de entrada fluem em apenas **uma direção**: das **entradas (inputs)** para as **saídas (outputs)**, passando por uma ou mais **camadas ocultas (hidden layers)**. Não há, em nenhum ponto da rede, conexões que retornem o sinal a camadas anteriores, o que a diferencia das **redes recorrentes (RNNs)**, nas quais há laços de realimentação temporal.

Em resumo, uma *Neural Network Feed-forward* é a base conceitual de toda a inteligência artificial moderna: um sistema matemático inspirado no cérebro humano, onde cada “neurônio” computa uma função simples, mas o conjunto, organizado em camadas, é capaz de representar funções de altíssima complexidade. É o modelo que transformou o aprendizado de máquina em aprendizado profundo, permitindo que computadores enxerguem, ouçam, interpretem e aprendam com dados do mundo real.

Em termos conceituais, uma rede neural feed-forward busca **aproximar uma função matemática** ( $f(x)$ ) capaz de mapear uma entrada ( x ) (um vetor de características) em uma saída ( y ) (uma predição). A rede aprende esse mapeamento ajustando parâmetros internos — os **pesos (weights)** e **biases (viéses)** — durante o processo de treinamento. O comportamento da rede é regido pela composição sucessiva de transformações lineares e não lineares, formalmente expressa por:

```math
a^{(l)} = f^{(l)}(W^{(l)} a^{(l-1)} + b^{(l)})
```

Onde ( $a^{(l)}$ ) é o vetor de ativações da camada ( l ), ( $W^{(l)}$ ) é a matriz de pesos que conecta a camada ( l-1 ) à camada ( l ), ( $b^{(l)}$ ) é o vetor de bias, e ( $f^{(l)}$ ) é a **função de ativação** (como ReLU, Sigmoid, ou Tanh), responsável por introduzir não linearidade — o que é essencial para que a rede aprenda funções complexas.

O processo de aprendizado de uma feed-forward network é dividido em duas fases principais. A primeira é a **forward propagation**, quando a entrada percorre as camadas e produz uma saída, permitindo comparar a resposta da rede com o valor esperado (rótulo). A diferença entre eles é o **erro** (ou *loss*), calculado por uma função de custo como o erro quadrático médio (MSE) ou a entropia cruzada (Cross-Entropy Loss). A segunda fase é a **backpropagation**, um algoritmo baseado na **regra da cadeia do cálculo diferencial** que propaga esse erro de volta pelas camadas, ajustando gradualmente os pesos por meio de um otimizador (geralmente o **Gradiente Descendente Estocástico — SGD**, ou variantes como Adam, RMSProp, Adagrad etc.). Esse ciclo se repete iterativamente até que a rede minimize o erro e aprenda os padrões dos dados.

A estrutura de uma rede feed-forward geralmente contém três tipos de camadas: uma **camada de entrada (input layer)**, que recebe os dados brutos; uma ou mais **camadas ocultas (hidden layers)**, que processam e transformam as informações; e uma **camada de saída (output layer)**, responsável por fornecer o resultado final. O número de camadas e neurônios define a **profundidade da rede**. Se houver muitas camadas ocultas, chamamos de uma **Deep Neural Network (DNN)** — que é, essencialmente, uma versão profunda da feed-forward clássica.

Um dos pilares teóricos que sustentam a importância das redes feed-forward é o **Teorema da Aproximação Universal**, que afirma que uma rede neural com apenas uma camada oculta e um número suficiente de neurônios pode aproximar qualquer função contínua em um intervalo compacto. Isso significa que, com parâmetros bem ajustados, uma feed-forward pode representar qualquer relação matemática entre entrada e saída, o que a torna uma poderosa ferramenta de modelagem.

Na prática, redes feed-forward são aplicadas em uma ampla gama de tarefas: desde problemas de **classificação supervisionada** (como reconhecimento de padrões, diagnósticos médicos ou categorização de texto), até **regressão** (como previsão de séries temporais, preços ou valores contínuos). Elas também servem de **bloco estrutural** para redes mais avançadas: as **redes convolucionais (CNNs)**, usadas em visão computacional, e os **transformers**, usados em processamento de linguagem natural, são derivações do modelo feed-forward, mas com mecanismos adicionais especializados.

Essa figura representa **uma rede neural profunda (Deep Learning Network)**, mais especificamente uma **rede neural feedforward de três camadas (Three-Layer Neural Network)**, que é uma das bases matemáticas do aprendizado profundo moderno. O diagrama mostra com detalhes o fluxo matemático entre as camadas de neurônios desde os vetores de entrada até as saídas, bem como as operações de pesos, vieses e funções de ativação que caracterizam o funcionamento interno de uma rede neural artificial.

![df6804dbaa3cd3a021bc462ce4be954d](https://github.com/user-attachments/assets/f0954b16-c0f3-483e-a473-6300930405ef)

Para compreender o que está acontecendo, vale lembrar que uma rede neural é essencialmente uma **função composta de várias funções não lineares**, aprendida a partir de dados. Cada camada aplica uma transformação linear (multiplicação de pesos e soma de vieses) seguida de uma transformação não linear (função de ativação). No diagrama, as fórmulas $a¹ = f¹(W¹p + b¹), a² = f²(W²a¹ + b²), e a³ = f³(W³a² + b³)$ descrevem precisamente esse processo. O vetor **p** representa o conjunto de entradas (features) com dimensão $R×1$. A matriz **W¹** contém os pesos que conectam as entradas aos neurônios da primeira camada, e **b¹** é o vetor de bias (viés) que desloca linearmente a saída da soma ponderada $Σ(Wp + b)$. A função $f¹$ representa a **função de ativação**, como ReLU, sigmoide, tanh ou softmax, dependendo do tipo de problema (classificação, regressão, etc.). Esse processo se repete nas camadas seguintes — cada saída a¹ alimenta a próxima camada como entrada, resultando em uma composição hierárquica de funções.

A grande sacada do **Deep Learning** está justamente nesse empilhamento de camadas. Cada camada aprende representações cada vez mais abstratas dos dados. Por exemplo, em uma rede treinada para reconhecimento de imagens, as primeiras camadas aprendem bordas e texturas, as intermediárias aprendem formas e padrões visuais, e as camadas mais profundas aprendem conceitos complexos como “rosto humano” ou “carro”. Essa hierarquia de abstração é o que torna o aprendizado profundo tão poderoso — a rede aprende automaticamente as features relevantes sem necessidade de engenharia manual de atributos.

Do ponto de vista matemático, a rede implementa uma composição de funções do tipo:

```math
a^3 = f^3(W^3 f^2(W^2 f^1(W^1 p + b^1) + b^2) + b^3)
```

Que é uma função altamente não linear. Durante o treinamento, o objetivo é ajustar os parâmetros (os pesos W e os vieses b) de forma que a saída da rede **minimize o erro** entre a predição e o valor real. Isso é feito com o **algoritmo de retropropagação (backpropagation)**, que calcula o gradiente do erro em relação a cada parâmetro e os atualiza na direção oposta do gradiente, seguindo a regra do **gradiente descendente** (gradient descent). A equação de atualização típica é:

```math
W_{ij}^{(t+1)} = W_{ij}^{(t)} - \eta \frac{\partial E}{\partial W_{ij}}
```

Onde ( $\eta$ ) é a taxa de aprendizado (learning rate) e ( $\frac{\partial E}{\partial W_{ij}}$ ) é o gradiente do erro em relação ao peso.

Portanto, sim: o diagrama que você mostrou é uma representação formal e simbólica de uma **Deep Neural Network (DNN)**, com três camadas ocultas e funções de ativação não lineares. Ela exemplifica como os dados são propagados (feedforward), transformados matematicamente e depois ajustados iterativamente pelo algoritmo de backpropagation. Essa estrutura é a base de praticamente todo o campo de Deep Learning — desde redes convolucionais (CNNs) em visão computacional até redes recorrentes (RNNs) e transformers usados em modelos de linguagem como o GPT.

Resumindo, essa rede é um **modelo de aprendizado profundo supervisionado**, estruturado para aprender funções complexas a partir de dados de entrada, e representa um dos pilares conceituais mais fundamentais da inteligência artificial moderna.

Uma **rede neural feedforward** é o tipo mais fundamental e conceitualmente puro de rede neural artificial. Ela é chamada assim porque a informação **flui apenas em uma direção** — do conjunto de entradas, passando pelas camadas ocultas, até chegar à camada de saída sem qualquer tipo de retroalimentação ou conexão cíclica entre os neurônios. Em termos formais, é uma função composta que transforma um vetor de entrada ( x ) em uma saída ( y ) por meio de várias transformações lineares seguidas de não linearidades. A ausência de ciclos é o que a distingue, por exemplo, das redes neurais recorrentes (RNNs), nas quais as saídas podem se realimentar como entradas para processar dados sequenciais.

Matematicamente, uma rede neural feedforward com ( L ) camadas pode ser representada como:

```math
a^{(L)} = f^{(L)}(W^{(L)} f^{(L-1)}(W^{(L-1)} f^{(L-2)}(\dots f^{(1)}(W^{(1)}x + b^{(1)}) \dots ) + b^{(L-1)}) + b^{(L)})
```

Onde ( $W^{(l)}$ ) é a matriz de pesos da camada ( $l$ ), ( $b^{(l)}$ ) é o vetor de bias, e ( $f^{(l)}$ ) é a função de ativação que introduz não linearidade. O objetivo do modelo é aprender os valores de ( W ) e ( b ) que minimizam uma função de erro (ou função de custo) ( $E$ ), como o erro quadrático médio (MSE) ou a entropia cruzada (Cross-Entropy Loss), dependendo do tipo de tarefa (regressão ou classificação).

A arquitetura básica de uma feedforward network tem três tipos de camadas principais:

<img height="177" align="right" src="https://github.com/user-attachments/assets/b8f2c38e-ea06-4d5b-8b18-9ee76d29e952" />

1. A **camada de entrada (input layer)** recebe os dados brutos (por exemplo, pixels de uma imagem, ou atributos numéricos de um dataset).

2. As **camadas ocultas (hidden layers)** são as responsáveis por aprender as representações intermediárias — elas aplicam transformações não lineares nos dados e combinam padrões mais simples para formar padrões mais complexos.

3. Por fim, a **camada de saída (output layer)** gera a predição final, que pode ser uma probabilidade (em problemas de classificação, por meio da função softmax) ou um valor contínuo (em regressão, com ativação linear).

O funcionamento do feedforward é dividido em duas fases principais. A primeira é a **propagação direta (forward propagation)**, onde o dado percorre toda a rede, camada por camada, até gerar a saída final. A segunda é o **aprendizado (treinamento)**, que utiliza o **algoritmo de retropropagação do erro (backpropagation)** combinado com um otimizador (como o gradiente descendente estocástico, Adam, RMSprop, etc.) para ajustar os pesos. Durante o backpropagation, o modelo aplica o **teorema da cadeia** para calcular os gradientes de cada parâmetro em relação ao erro final e atualizá-los proporcionalmente.

O propósito de uma rede feedforward é **aproximar funções não lineares complexas**. Segundo o **Teorema da Aproximação Universal**, uma rede neural com apenas uma camada oculta e número suficiente de neurônios pode aproximar qualquer função contínua em um domínio compacto. Isso significa que, teoricamente, mesmo uma rede simples pode aprender relações arbitrariamente complexas entre entrada e saída, embora na prática redes mais profundas (com várias camadas ocultas) sejam necessárias para capturar relações hierárquicas e reduzir a dimensionalidade de forma eficiente.

Em termos práticos, redes feedforward são amplamente utilizadas em problemas de classificação (como reconhecimento de dígitos, diagnóstico médico, ou detecção de fraudes), regressão (previsão de preços ou séries temporais) e também como blocos básicos em arquiteturas mais avançadas, como as **redes convolucionais (CNNs)** e os **transformers**. Embora sejam a forma mais “simples” de rede neural, elas são conceitualmente o núcleo de toda a inteligência artificial moderna — cada tipo de rede mais sofisticado (como RNN, CNN, LSTM, GAN ou Transformer) é, em essência, uma generalização do modelo feedforward.

Portanto, uma **rede neural feedforward** é uma estrutura matemática de aprendizado supervisionado que processa dados em uma única direção — da entrada à saída —, aprendendo a mapear padrões complexos por meio de ajustes iterativos nos pesos sinápticos, funcionando como um sistema de aproximação universal de funções e base teórica do aprendizado profundo.

## [DL] CNNs - Convolutional Neural Networks
<img height="77" align="right" src="https://github.com/user-attachments/assets/0fdd400c-87e7-452e-a48d-37c64e5523d4" />

As **CNNs - Convolutional Neural Networks** são uma das arquiteturas mais influentes do deep learning porque conseguiram capturar, de forma quase orgânica, a maneira como a informação visual realmente se organiza no espaço. 

Diferente de um MLP tradicional, que tenta aprender padrões olhando para todos os pixels ao mesmo tempo como se cada pedaço da imagem fosse igualmente relevante, uma CNN adota a lógica da visão natural: ela enxerga pedaços pequenos, reconhece neles estruturas simples e, camada após camada, constrói significados mais complexos a partir dessas peças fundamentais. É como se a rede imitasse o processo do sistema visual humano, começando com a detecção de bordas e contrastes e terminando na compreensão de objetos inteiros.

CNN (Rede Neural Convolucional) é a espinha dorsal da visão computacional. Até mesmo algoritmos de detecção de objetos, como o RCNN mais rápido, dependem da CNN para realizar sua tarefa. Portanto, ter um bom entendimento de CNN ajuda você a se destacar na área de visão computacional. Usaremos a CNN para realizar a classificação de imagens. Vou compartilhar o código padrão que você pode reutilizar.

O coração dessa arquitetura está no processo de convolução, em que pequenos filtros — matrizes de pesos — deslizam sobre a imagem examinando regiões locais. Cada filtro aprende a destacar algo diferente: um pode responder a uma borda vertical, outro a uma textura pontilhada, outro a uma curva suave. Isso cria uma espécie de mapa de ativação, onde cada região da imagem revela “o quanto” aquele padrão está presente ali. O efeito disso é uma rede com uma sensibilidade espacial muito precisa, capaz de reconhecer o mesmo padrão independentemente de onde ele esteja. Essa propriedade, chamada invariância translacional, é exatamente o que torna CNNs tão poderosas para análise de imagens.

Conforme as camadas avançam, surge um efeito de composição hierárquica. As primeiras camadas aprendem estruturas elementares; as intermediárias combinam essas estruturas em formas maiores, como cantos, partes de objetos ou padrões repetitivos; e as mais profundas passam a reconhecer conceitos inteiros. É por isso que, em redes profundas como a ResNet ou a Inception, os mapas de ativação finais respondem claramente a categorias visuais como `“gato”`, `“roda”`, `“janela”`, `“pata”`, `“farol”`. A rede não memoriza imagens: ela aprende representações cada vez mais abstratas e semânticas daquilo que vê.

Exemplo:

<img width="720" height="235" alt="image" src="https://github.com/user-attachments/assets/12335839-15ca-4edd-81a1-635918c3295c" />

Outro elemento importante é o pooling, que reduz progressivamente a resolução espacial da imagem enquanto preserva a informação essencial. Isso dá à rede uma espécie de visão panorâmica gradual, condensando detalhes em estruturas mais compactas. O resultado é uma arquitetura que consegue ver tanto o micro quanto o macro ao mesmo tempo, equilibrando detalhe e contexto.

<img height="177" align="right" src="https://github.com/user-attachments/assets/887d5e08-8baf-4a69-a479-057fc55b0fdf" />

CNNs mudaram todo o campo da visão computacional e permitiram avanços que antes eram impossíveis. Elas se tornaram a base de sistemas de reconhecimento facial, diagnóstico médico por imagem, carros autônomos, análise de satélite, detecção de objetos em tempo real, segmentação de cenas, reconstrução e restauração visual. Modelos clássicos como AlexNet, VGG, ResNet, MobileNet e EfficientNet não apenas dominaram benchmarks como o ImageNet, mas redefiniram o que significa “ver por meio de algoritmos”.

Mesmo com o crescimento dos Transformers aplicados a visão, as CNNs continuam extremamente relevantes, especialmente quando se precisa de precisão espacial, eficiência, robustez ou quando os dados têm uma estrutura física clara no espaço. 

Arquiteturas híbridas modernas combinam convolução com atenção exatamente porque as CNNs capturam relações locais com uma naturalidade que ainda não foi substituída por completo. Em essência, uma CNN é uma homenagem matemática ao próprio ato de enxergar: fragmentos locais que, somados e reinterpretados em camadas sucessivas, formam a compreensão global do mundo visual.

![616136998_1353369200138234_7703530091595592433_n](https://github.com/user-attachments/assets/b5f06cf6-d825-4346-9809-21923151efce)

O primeiro passo é importar as bibliotecas necessárias. As bibliotecas facilitam nossa vida, pois não precisamos implementá-las do zero:

```python
import os
import numpy as np
import tensorflow as tf
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense, Conv2D, Flatten, Dropout, MaxPooling2D
from tensorflow.keras.preprocessing.image import ImageDataGenerator
```

Certifique-se de instalar as bibliotecas caso apresente algum erro ao importar.

Processamento de dados: A estrutura do meu diretório é a seguinte:

```
images
   |____train
   |       |___class A
   |       |___class B
   |       |___class C
   |
   |-----test
   |       |___class A
   |       |___class B
   |       |___class C
```

## [DL] GANs - Generative Adversarial Networks
<img src="https://github.com/user-attachments/assets/bd796821-006c-471d-981e-d1e8c09f172a" align="right" height="77">

As **GANs - Generative Adversarial Networks** representam uma das ideias mais elegantes e revolucionárias da história do deep learning, e talvez a mais “viva” delas, porque surgem não como um modelo isolado, mas como um sistema composto de duas redes que aprendem em confronto direto, quase como duas inteligências artificiais em duelo. 

A essência das GANs é simples, mas profundamente poderosa: uma rede, chamada gerador, tenta criar dados sintéticos que pareçam reais; a outra, chamada discriminador, tenta detectar se aquilo que recebeu é verdadeiro ou falso. Esse jogo de gato e rato faz com que o gerador aprenda gradualmente não apenas a imitar padrões superficiais, mas a capturar estruturas inteiras de distribuição de dados, resultando em imagens, sons ou textos que parecem emergir de um processo autêntico e natural.

O gerador começa produzindo lixo — ruído puro, sem forma e sem sentido — mas, a cada rodada, o discriminador o expõe, aponta os erros, indica onde a ilusão falhou. Essa crítica é enviada de volta ao gerador por meio do gradiente, que ajusta seus parâmetros para melhorar a próxima tentativa. O discriminador, por sua vez, também melhora, aprendendo a reconhecer enganações cada vez mais sofisticadas. O jogo, então, fica mais refinado, mais tenso, mais sutil. 

Eventualmente, chega um ponto em que o gerador consegue produzir resultados tão convincentes que o discriminador fica quase indiferente: não há mais gordura aparente, não há mais marcas óbvias do artificial, e o sistema atinge um tipo de equilíbrio delicado chamado de Nash. O fascinante é que esse equilíbrio não é estável — é mais como um momento de trégua — mas é justamente nesse momento que nascem as melhores criações.

A força das GANs está na capacidade de modelar distribuições de probabilidade extremamente complexas sem necessidade de definir funções explícitas para isso. Em vez de um modelo que tenta se aproximar diretamente dos dados, as GANs aprendem a *produzir* amostras da mesma forma que esses dados são originados. Isso permite gerar rostos que nunca existiram, criar pinturas no estilo de artistas mortos há séculos, sintetizar vozes, ampliar imagens sem perda aparente de qualidade, criar mundos inteiros para simulações, restaurar fotos antigas, simular moléculas, gerar datasets para treinar outros modelos e até compor músicas. Não é exagero dizer que GANs inauguraram a era moderna da geração artificial criativa.

Mas essa elegância vem com desafios profundos. GANs são notoriamente difíceis de treinar, porque o equilíbrio entre gerador e discriminador é frágil. Se o discriminador fica forte demais, o gerador não aprende nada; se o gerador domina rápido demais, o discriminador fica cego. Além disso, há o problema do mode collapse, onde o gerador aprende a produzir apenas um subconjunto muito pequeno da distribuição esperada, gerando amostras repetitivas que enganam o discriminador, mas não representam a diversidade dos dados originais. 

![unnamed](https://github.com/user-attachments/assets/1d7e4f7c-63a3-41d9-ba5a-52f15178322b)

<img width="450" height="450" alt="brainstorming-3d-icon-download-in-png-blend-fbx-gltf-file-formats--idea-business-teamwork-management-pack-icons-7479918" src="https://github.com/user-attachments/assets/e88d91e4-beab-4926-93c5-f893fac93d20" />

Resolver esses problemas levou a variações inteiras — WGANs, StyleGAN, CycleGAN, BigGAN, ProGAN — cada uma refinando algum aspecto do jogo adversarial. E, embora transformers tenham avançado no território da geração multimodal, as GANs continuam insuperáveis em fidelidade visual, textura, nitidez e controle fino da estética.

<img width="200" height="200" alt="brain-inside-lightbulb-3d-render-on-transparent-background-png" src="https://github.com/user-attachments/assets/964c412c-cf94-47e1-899c-733c9231fcb6" />

Em última análise, GANs são menos um algoritmo e mais uma metáfora matemática para como criatividade pode emergir de tensão. Duas forças opostas, alinhadas pela retropropagação, produzem algo que nenhuma delas conseguiria conceber sozinha. É como se a verdade e a mentira, em conflito permanente, acabassem parindo uma nova forma de realidade — sintética, sim, mas tão detalhada e coerente que se torna quase indistinguível da original.

<img width="980" height="980" alt="innovation-concept-with-brain-in-bulb-lamp-3d-icon-free-png" src="https://github.com/user-attachments/assets/449f9fe1-56bd-4eaf-9221-894d35587726" />

## [DL] RNN - Recurrent Neural Networks
<a href=""><img src="https://img.shields.io/badge/Python-NN-FFD21E?style=flat&logo=Python&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/R-NN-FFD21E?style=flat&logo=R&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Tensorflow-NN-FFD21E?style=flat&logo=Tensorflow&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Pytorch-NN-FFD21E?style=flat&logo=Pytorch&logoColor=white"></a> <a href="https://www.youtube.com/@PROFESSORKENNYOFICIAL"><img src="https://img.shields.io/badge/Keras-NN-tomato?style=flat&logo=Keras&logoColor=white"></a> <a href="https://notebooklm.google/"><img src="https://img.shields.io/badge/GCP-NN-tomato?style=flat&logo=googlecloud&logoColor=white"></a>

<img height="477" align="right" src="https://github.com/user-attachments/assets/27a22a23-7c66-48d1-a46d-529fb4f415df" />

As **Redes Neurais Recorrentes** (RNN - Recurrent Neural Networks), representam uma classe fundamental de arquiteturas de redes neurais projetadas especificamente para processar dados sequenciais, quebrando uma limitação crucial das redes feedforward tradicionais. 

Enquanto uma rede neural convencional trata cada entrada como independente, assumindo que não há relação entre uma palavra em um texto, um frame em um vídeo ou uma amostra em uma série temporal, as RNNs introduzem uma noção de "memória" ao manter um estado interno que é atualizado a cada passo de uma sequência. Esta característica as torna biologicamente mais plausíveis e computacionalmente mais adequadas para tarefas onde o contexto e a ordem dos elementos são informativos, se não críticos, para a interpretação correta.

O mecanismo central que permite essa memória é o **loop de feedback** presente em sua unidade básica. Imagine uma célula RNN como uma caixa que recebe duas entradas em cada passo de tempo `t`: a entrada atual `x_t` (como uma palavra em uma frase) e um **estado oculto** `h_{t-1}`, que é uma representação compacta de tudo o que a rede "viu" nos passos anteriores. Internamente, a célula combina essas duas entradas, aplica transformações (geralmente envolvendo pesos treináveis e uma função de ativação como `tanh`), e produz duas saídas: um estado oculto atualizado `h_t` que será repassado para o próximo passo da sequência, e uma saída `y_t` que pode ser usada para uma previsão naquele instante. Este ciclo de alimentar o estado anterior de volta na rede é o que cria a dependência temporal e permite que a informação teoricamente flua indefinidamente ao longo da sequência.

Esta arquitetura torna as RNNs notavelmente versáteis e aplicáveis a uma gama impressionante de domínios. No Processamento de Linguagem Natural, elas foram a base para modelagem de linguagem, tradução automática e análise de sentimentos, onde o significado de uma palavra depende fortemente das que a precederam. No reconhecimento de fala, elas podem modelar a dependência temporal entre frames de áudio. Para a previsão de séries temporais — de preços de ações a consumo de energia —, a RNN pode aprender padrões complexos e sazonais nos dados históricos para prever valores futuros. E na geração de sequências, uma RNN treinada em um corpus de texto pode produzir novo texto caractere por caractere ou palavra por palavra, com uma coerência contextual surpreendente.

No entanto, a arquitetura RNN clássica sofre de um problema teórico e prático severo conhecido como o **problema do vanishing/exploding gradient**. Durante o treinamento por retropropagação através do tempo, os gradientes — que são os sinais que indicam como ajustar os pesos da rede — são multiplicados repetidamente através de cada passo da sequência. Se esses gradientes forem sistematicamente menores que 1, eles encolhem exponencialmente até desaparecerem, tornando a rede incapaz de aprender dependências de longo prazo. Se forem sistematicamente maiores que 1, eles explodem, tornando o treinamento instável. Esta limitação fundamental significa que, na prática, as RNNs simples têm grande dificuldade em capturar contextos que se estendem por mais de alguns passos.

Foi precisamente para superar essa barreira que arquiteturas mais sofisticadas foram desenvolvidas, sendo as mais notáveis a **Long Short-Term Memory (LSTM)** e a **Gated Recurrent Unit (GRU)**. Essas variantes introduzem um mecanismo inteligente de "portas" que atuam como interruptores regulados para controlar com precisão qual informação deve ser mantida no estado de longo prazo, qual deve ser esquecida e qual deve ser expelida como saída. A LSTM, com sua célula de memória e portas de entrada, esquecimento e saída, tornou-se o trabalho padrão para a maioria das aplicações sequenciais complexas por muitos anos, demonstrando uma capacidade muito superior de reter informações relevantes ao longo de centenas ou mesmo milhares de passos de tempo.

Em resumo, as Redes Neurais Recorrentes representam um marco conceitual no deep learning, pois foram as primeiras a modelar formalmente a dimensão do tempo e da ordem. Embora suas formas mais simples tenham sido em grande parte suplantadas pelas LSTMs, GRUs e, mais recentemente, pelos Transformers para muitas tarefas, a ideia central da recorrencia — que o estado passado deve influenciar o processamento presente — permanece uma intuição profunda e indispensável. Elas pavimentaram o caminho para que máquinas não apenas processassem pixels ou tokens isolados, mas começassem a compreender e gerar narrativas, músicas, discursos e tendências que se desdobram no tempo, capturando um aspecto fundamental da inteligência e da experiência humana.

## [DL] RBFNs - Radial Basis Function Networks
<img height="77" align="right - Copia" src="https://github.com/user-attachments/assets/de9e6b8a-f4bb-4e26-bf36-176719d10ed7" />

As **RBFNs - Radial Basis Function Networks** representam uma das alternativas mais elegantes e matematicamente limpas às redes neurais tradicionais baseadas em camadas densas. Enquanto um MLP tenta aprender a relação entrada-saída ajustando pesos em todas as direções ao mesmo tempo, uma RBFN funciona como uma espécie de mapa de influências locais espalhadas pelo espaço de entrada. Cada neurônio da camada escondida não aprende um peso, mas sim um “centro” — um ponto no espaço onde sua resposta é máxima — e uma “largura” que determina o quão longe sua influência alcança. A ativação típica é uma função radial, quase sempre uma gaussiana, que diminui suavemente à medida que os dados se afastam desse centro. Isso cria uma paisagem de pequenas montanhas matemáticas que, combinadas, conseguem aproximar praticamente qualquer função de maneira muito suave e controlada.

O funcionamento de uma RBFN é dividido em duas etapas conceituais: primeiro, os centros das funções radiais são definidos, muitas vezes por clustering (como K-means), o que significa que a rede literalmente organiza as regiões do espaço onde os dados se agrupam. Depois disso, a camada de saída aprende apenas uma combinação linear dessas bases radiais. É como se a rede decidisse: “aqui está uma coleção de sinos gaussianos posicionados onde os dados acontecem; agora, basta descobrir como somá-los para reproduzir a função desejada”. Isso deixa o processo de aprendizagem muito mais estável e menos dependente de correções infinitas de gradiente como acontece em MLPs.

O caráter local das ativações radiais faz com que as RBFNs sejam particularmente boas para problemas onde a relação entre entrada e saída depende fortemente de proximidade. Classificações com fronteiras complexas e não lineares, interpolação suave de dados, sistemas com comportamento regionalizado e até aproximações funcionais clássicas se beneficiam desse tipo de arquitetura. Em essência, elas criam uma espécie de “atlas” do espaço, onde cada neurônio é responsável por uma vizinhança específica, evitando o excesso de interferência global que um MLP pode introduzir.

Apesar de serem menos populares que redes profundas modernas, elas permanecem extremamente úteis em contextos onde interpretabilidade, estabilidade e precisão local importam mais do que escalabilidade extrema. Elas também servem de ponte conceitual entre as redes neurais e métodos baseados em kernels, como SVM com kernel gaussiano, já que ambos compartilham a ideia de construir soluções a partir de funções de base centradas em pontos estratégicos. Dessa forma, as RBFNs mostram como a inteligência artificial pode emergir não apenas da profundidade, mas da forma como o espaço é organizado e de como a proximidade pode ser transformada em significado matemático.

## [DL] MLPs - Multilayer Perceptrons
<img src="https://github.com/user-attachments/assets/62c26363-63ec-42bb-b40d-fe0d804a834a" align="right" height="277">

Os **MLPs - Multilayer Perceptrons** são a forma mais clássica, fundamental e “canônica” de rede neural artificial, praticamente o ponto de partida conceitual para tudo que veio depois em deep learning. Um MLP é, essencialmente, uma pilha de camadas totalmente conectadas, onde cada neurônio recebe entradas ponderadas, soma tudo, adiciona um viés e aplica uma função de ativação não linear. O grande insight é exatamente essa não linearidade: ela permite que a rede deixe de ser apenas uma planilha glorificada de multiplicações e se torne uma máquina capaz de aproximar funções altamente complexas. A arquitetura é simples, uma camada de entrada, uma ou mais camadas escondidas e uma camada de saída, mas essa simplicidade esconde um poder matemático muito profundo.

A ideia fundamental do MLP é aprender uma função ( $f(x)$ ) capaz de mapear entradas para saídas desejadas, e isso é feito ajustando pesos e vieses via backpropagation, que, por sua vez, utiliza um otimizador como gradiente descendente ou variantes mais modernas (Adam, RMSProp, etc.). O treinamento funciona como um ciclo de tentativa e erro, em que a rede faz uma previsão, compara com o valor verdadeiro, calcula o erro e empurra esse erro de volta pelas camadas para corrigir os pesos. Com repetições suficientes, o MLP converge para um conjunto de parâmetros que capturam as regularidades essenciais do problema. É um processo quase darwinista, onde cada ajuste microscópico melhora a capacidade da rede de “entender” o padrão subjacente.

O MLP é versátil porque se adapta a praticamente qualquer tipo de tarefa supervisionada tradicional: classificação, regressão e até algumas formas de previsão temporal quando combinado com janelas deslizantes. Embora outras arquiteturas especializadas — CNNs para visão, RNNs e Transformers para sequências — dominem seus respectivos campos, os MLPs continuam relevantes não só como modelos leves e eficientes, mas também como blocos conceituais que explicam como redes mais elaboradas funcionam. Muita coisa em deep learning é, na essência, um grande MLP reorganizado com estruturas especiais. Além disso, MLPs modernos, quando ampliados com camadas residuais, normalização e ativadores avançados, reaparecem até mesmo dentro dos Transformers, onde servem como o “miolo” das camadas feed-forward. Ou seja, apesar de serem uma das primeiras formas de rede neural, continuam formando o esqueleto intelectual da maior parte das técnicas usadas atualmente.

## [DL] SOMs - Self Organizing Maps
<img src="https://github.com/user-attachments/assets/ccd5407c-d9e0-4303-b1fe-1b33564f8663" align="right" height="77">

As **SOMs - Self-Organizing Maps** são um tipo de rede neural não supervisionada criada por Teuvo Kohonen nos anos 1980, e o próprio nome já revela a natureza do processo: trata-se de um mapa que se organiza sozinho a partir dos padrões existentes nos dados. A lógica central por trás de um SOM não é prever uma saída específica nem classificar algo a partir de rótulos conhecidos, mas aprender a estrutura interna de um conjunto de dados de forma puramente observacional. 

Ele pega dados que normalmente estão espalhados em um espaço de alta dimensionalidade e tenta projetar esses dados em um mapa bidimensional onde pontos semelhantes ficam próximos e pontos diferentes ficam afastados. É como se fosse uma espécie de topografia neuronal que tenta “achatar” mundos complexos para que a tua percepção do agrupamento real apareça naturalmente.

O princípio fundamental é o do “vencedor leva tudo”. Cada unidade do mapa é representada por um vetor de pesos, e quando um dado de entrada chega, a rede procura qual desses neurônios tem pesos mais parecidos com esse dado. Esse neurônio é chamado de Best Matching Unit, ou BMU. Uma vez encontrado o BMU, não é apenas ele que é ajustado; toda uma vizinhança ao redor dele também é atualizada, de modo a tornar o mapa mais suave, mais coerente topologicamente, e mais fiel à distribuição real dos dados. Isso cria uma dinâmica onde o mapa inteiro vai gradualmente se moldando à geometria estatística da entrada, formando regiões que espontaneamente capturam similaridades e clusters, mesmo sem alguém ter dito à rede quais eram esses clusters. Por isso os SOMs são tão usados em visualização de dados, redução de dimensionalidade e descoberta de padrões ocultos.

Com o tempo, conforme as iterações acontecem, a vizinhança de atualização encolhe e a taxa de aprendizado diminui. No começo, o mapa inteiro se mexe agressivamente, como um tecido esticado tentando se ajustar à forma de um objeto. Na fase final, ele se torna mais rígido, refinando detalhes e criando fronteiras mais nítidas entre os grupos. Isso faz com que o SOM seja particularmente interessante para campos como análise exploratória de dados, mineração de padrões, compressão de informação e até mesmo organização semântica em domínios como processamento de linguagem natural. Ele não substitui métodos mais modernos como t-SNE ou UMAP quando o foco é puramente visual, mas ainda assim SOMs mantêm relevância por combinar interpretabilidade, estabilidade e a capacidade de manter relações topológicas que muitas técnicas mais recentes simplesmente descartam.

É uma ferramenta clássica de deep learning antes mesmo de deep learning virar a tempestade moderna que conhecemos, e continua sendo um exemplo elegante de como redes neurais podem aprender apenas observando, sem que ninguém lhes diga o que é certo ou errado.

## [DL] DBNs - Deep Belief Networks
<img height="77" align="right" src="https://github.com/user-attachments/assets/ac7ecd7f-b487-4c1f-aef1-df79f8f72027" />

As **Deep Belief Networks (DBNs)** são modelos fundamentais no período inicial da história moderna do Deep Learning, representando uma ponte entre as redes neurais profundas clássicas e os modelos generativos contemporâneos. Uma DBN é, essencialmente, uma arquitetura probabilística composta por múltiplas camadas empilhadas de modelos chamados **Restricted Boltzmann Machines (RBMs)**, funcionando de maneira hierárquica, onde cada camada aprende representações cada vez mais abstratas dos dados. Embora hoje elas tenham sido amplamente substituídas por arquiteturas mais eficientes e treinamentos end-to-end, como autoencoders variacionais, GANs e modelos baseados em transformadores, a ideia por trás das DBNs continua influenciando várias técnicas de aprendizado profundo e permanece como um marco conceitual.

Para entender uma DBN, é importante compreender que, antes de 2006, redes neurais profundas eram quase impossíveis de treinar de forma eficiente, principalmente por causa do problema do gradiente que desaparece. Treinar muitas camadas com backpropagation levava a mínimos ruins, perda de informação ao longo das camadas e resultados decepcionantes. Hinton propôs uma solução engenhosa: em vez de tentar treinar toda a rede de uma vez, poderia-se treinar cada camada separadamente usando uma RBM, um modelo generativo não supervisionado capaz de aprender distribuições de probabilidade sobre seus dados de entrada. Esse processo, chamado **pretreinamento camada a camada**, permitia que cada parte da rede aprendesse uma estrutura interna consistente antes de ser combinada na rede profunda completa. Era como esculpir cada andar de um edifício separadamente, garantindo estabilidade estrutural, para só depois unir as partes e finalizar o acabamento.

A lógica interna é fascinante. A camada mais baixa aprende padrões diretos dos dados brutos: bordas, texturas iniciais, variações simples. A segunda camada aprende padrões das ativações da primeira, captando combinações mais ricas e abstratas. Conforme as camadas avançam, os padrões se tornam mais sofisticados e menos intuitivos para o olhar humano, representando características latentes complexas da distribuição. Essa hierarquia de abstração, hoje comum em redes convolucionais e transformers, foi uma das primeiras provas práticas de que representações profundas podiam ser aprendidas de maneira eficiente e progressiva. A DBN, portanto, inaugurou a noção moderna de profundidade como mecanismo de aprendizado hierárquico.

Depois que todas as RBMs eram treinadas individualmente, vinha a etapa final: ajustar toda a rede como um modelo discriminativo ou gerativo, usando backpropagation tradicional, agora partindo de pesos muito mais bem posicionados. Isso aumentava drasticamente a qualidade do aprendizado supervisionado, evitando que o modelo ficasse preso em mínimos ruins. Foi esse mecanismo de pretreinamento que marcou 2006 como o ano do “renascimento das redes neurais profundas”, abrindo caminho para uma década de explosão em técnicas de Deep Learning.

Em essência, uma Deep Belief Network é um **modelo híbrido**, combinando características generativas e discriminativas. Em suas camadas superiores, ela funciona como um modelo gráfico probabilístico, capturando relações estocásticas complexas entre variáveis ocultas. Nas camadas inferiores, ela atua quase como uma rede neural tradicional, transformando entradas de maneiras úteis para tarefas supervisionadas. Essa mistura fez das DBNs um modelo versátil para tarefas como reconhecimento de padrões, classificação, compressão de informação e aprendizado de características a partir de dados não rotulados, uma capacidade extremamente relevante em períodos onde datasets gigantescos eram menos comuns.

Com o avanço das técnicas modernas, as DBNs acabaram saindo do uso mainstream porque eram difíceis de escalar, exigiam treinamento delicado, sofriam com limitações teóricas e práticas das RBMs e não competiam bem com arquiteturas mais eficientes como CNNs profundas, LSTMs avançados ou transformers. Porém, historicamente, elas foram a prova de conceito que demonstrou que profundidade podia ser treinada com estabilidade, inaugurando a era do Deep Learning como conhecemos. Elas também estabeleceram princípios centrais como aprendizado não supervisionado para inicialização de redes, decomposição hierárquica de padrões e uso de modelos energéticos.

Em outras palavras, as DBNs são menos importantes hoje como ferramenta prática e mais importantes como marco conceitual: foram uma das primeiras arquiteturas capazes de revelar que redes profundas não eram apenas possíveis, mas incrivelmente poderosas quando bem construídas e bem iniciadas. Sem elas, o salto para os modelos modernos teria sido muito mais lento.

## [DL] RBMs - Restricted Boltzmann Machines
<img src="https://github.com/user-attachments/assets/6eb56e88-0f89-4269-8006-ccb1068e2366" align="right" height="177">

Uma **Restricted Boltzmann Machine (RBM)** é um tipo de rede neural probabilística e não supervisionada usada para aprender representações internas (features latentes) de dados. Ela foi muito importante na história do Deep Learning, especialmente entre 2006 e 2014, antes do domínio dos modelos modernos baseados em transformadores, mas ainda é um conceito fundamental em modelos generativos clássicos.

Uma RBM é formada por duas camadas: a camada visível e a camada oculta. A camada visível recebe os dados de entrada, enquanto a camada oculta aprende padrões internos sobre esses dados. A grande característica estrutural da RBM é que não existem conexões dentro de uma mesma camada; ou seja, neurônios visíveis não se conectam entre si, e neurônios ocultos também não se conectam entre si. Isso reduz drasticamente a complexidade matemática da rede e permite derivar probabilidades fechadas para ativação de cada neurônio. As RBMs são modelos **energéticos**, ou seja, elas não aprendem minimizando erro diretamente como redes convencionais, mas aprendem ajustando seus pesos para que o modelo associe menor “energia” a configurações de entrada que façam sentido e maior energia a configurações improváveis. Essa ideia vem da Física Estatística, especialmente do modelo de Ising; a função de energia define o quanto uma configuração visível-oculta é compatível com o que o modelo aprendeu, e a distribuição de probabilidade associada a essa energia segue a distribuição de Boltzmann, daí o nome.

O aprendizado nas RBMs ocorre por um processo chamado *Contrastive Divergence* (CD), criado por Geoffrey Hinton. Em termos simples, o algoritmo pega uma amostra real, calcula como os neurônios ocultos deveriam ser ativados, e depois reconstrói a entrada passando novamente pela rede. A atualização dos pesos é baseada na diferença entre a correlação visível-oculta das amostras reais e das amostras reconstruídas. É uma forma aproximada de maximizar a verossimilhança do modelo, evitando cálculos computacionalmente impossíveis como a partição exata da distribuição. Na prática, isso permite que a RBM aprenda a extrair padrões importantes do conjunto de dados de maneira não supervisionada, funcionando como um “compressor” probabilístico de informações.

RBMs ficaram famosas porque serviam como blocos construtivos para **Deep Belief Networks (DBNs)** e foram um marco inicial do renascimento do Deep Learning em 2006, quando Hinton mostrou que pilhas de RBMs podiam ser pré-treinadas camada a camada para depois serem refinadas supervisionadamente, superando redes neurais profundas que naquela época sofriam com gradientes que desapareciam. Em visão computacional, recomendação e redução de dimensionalidade, elas chegaram a ser muito usadas, e até hoje ainda aparecem em pesquisa acadêmica por sua capacidade generativa. Apesar de terem sido amplamente substituídas por autoencoders variacionais, GANs e transformadores modernos, elas permanecem como um conceito teórico importante porque introduziram estruturas probabilísticas em redes neurais e influenciaram a arquitetura de vários modelos subsequentes.

Em termos intuitivos, uma RBM aprende a responder perguntas do tipo: “dado esse padrão visível, quais representações internas o descrevem melhor?” e “dado essas representações internas, qual padrão visível deveria ser reconstituído?”. Ela é como um mecanismo que aprende distribuições de probabilidade de alto nível no espaço dos dados, criando uma espécie de mapa energético que distingue combinações comuns das incomuns. Essa perspectiva baseada em energia é justamente o ancestral direto dos Energy-Based Models modernos.

## [DL] Autoencoders
<img src="https://github.com/user-attachments/assets/30b79b23-1728-4e43-9b63-a0772b822923" align="right" height="77">

**Autoencoders** são um tipo especial de rede neural dentro do campo do *Deep Learning*, projetado para aprender representações compactas e eficientes dos dados, ou seja, para comprimir e reconstruir informações. 

A ideia central é simples, mas poderosa: treinar a rede para que ela receba uma entrada (por exemplo, uma imagem, som, texto ou vetor numérico), a comprima em uma forma reduzida chamada **codificação** ou **representação latente** e depois tente **reconstruir a entrada original** a partir dessa versão comprimida. Assim, o autoencoder aprende uma forma de representação interna que captura a essência dos dados, eliminando ruídos e redundâncias.

Tecnicamente, um autoencoder é composto por duas partes simétricas: o **encoder** e o **decoder**. O *encoder* (ou codificador) é responsável por transformar os dados de entrada ( x ) em uma forma comprimida ( z ), geralmente de menor dimensionalidade, através de uma função não linear ( $z = f(Wx + b)$ ). Essa etapa busca representar o conteúdo essencial da entrada em um espaço latente — um espaço vetorial abstrato onde informações semelhantes ficam próximas. 

Já o *decoder* (ou decodificador) faz o caminho inverso: ele tenta reconstruir a entrada original a partir de ( z ), gerando ( $\hat{x} = g(W'z + b')$ ). O objetivo do treinamento é minimizar a diferença entre ( x ) e ( $\hat{x}$ ), normalmente utilizando uma função de erro como o **Mean Squared Error (MSE)**:

```math
L = ||x - \hat{x}||^2
```

A minimização dessa função força a rede a aprender a codificar e decodificar a informação de forma eficiente.

O ponto interessante é que os autoencoders **não aprendem rótulos** (labels) — ou seja, são modelos **não supervisionados**. Eles aprendem puramente a partir da estrutura dos dados. Isso os torna extremamente úteis em tarefas como **redução de dimensionalidade**, **detecção de anomalias**, **remoção de ruído (denoising)**, **compressão de imagens** e **pré-treinamento de redes neurais profundas**. 

Por exemplo, em vez de usar PCA (Principal Component Analysis) para reduzir a dimensionalidade de um conjunto de imagens, um autoencoder pode aprender representações muito mais ricas e não lineares.

Com o avanço do Deep Learning, surgiram variações sofisticadas de autoencoders. Os **Denoising Autoencoders** são treinados para reconstruir entradas corrompidas, o que os torna robustos a ruídos. Os **Sparse Autoencoders** impõem restrições para que apenas alguns neurônios sejam ativados, o que força a rede a encontrar padrões mais significativos. E os **Variational Autoencoders (VAEs)** são uma evolução probabilística: em vez de gerar apenas uma codificação fixa, eles aprendem uma **distribuição latente** — uma representação estatística contínua dos dados. Isso permite gerar novas amostras semelhantes às do conjunto original, sendo um pilar fundamental da **aprendizagem generativa** (junto com os GANs, Generative Adversarial Networks).

Conceitualmente, os autoencoders são como uma forma de **autoanálise dos dados**: o sistema olha para si mesmo e aprende a descrever sua própria estrutura interna, sem precisar que alguém lhe diga o que procurar. Essa capacidade de **auto-representação** é uma das bases mais elegantes e matematicamente fascinantes do Deep Learning — uma verdadeira ponte entre compressão de informação, estatística e cognição artificial.

## [DL] Transformer
<img src="https://github.com/user-attachments/assets/aba9bc51-110f-4b10-ab5f-6670cdb089fe" height="177" align="right">

O **Transformer** é um modelo de aprendizado de máquina que revolucionou o campo do processamento de linguagem natural (NLP) e outras áreas de aprendizado de máquina. Ele foi apresentado pela primeira vez em 2017 por Ashish Vaswani et al. no artigo "Attention Is All You Need". Todos os modelos Transformer são uma forma de Deep Learning que por sua vez todos os modelos Transformer são uma forma de aprendizado de máquina (Machine Learning). Eles são projetados para aprender padrões e relações em dados, e para realizar tarefas como classificação, regressão, geração de texto, tradução automática, entre outras.

Um modelo transformer é uma rede neural que aprende o contexto e, assim, o significado com o monitoramento de relações em dados sequenciais como as palavras desta frase. Os modelos transformer aplicam um conjunto em evolução de técnicas matemáticas, chamadas de atenção ou autoatenção, para detectar as maneiras sutis como até mesmo elementos de dados distantes em uma série influenciam e dependem uns dos outros.

Descritos pela primeira vez em um artigo de 2017 do Google, os transformers estão entre os modelos mais novos e potentes já inventados até hoje. Eles estão impulsionando uma onda de avanços em machine learning, o que alguns chamam de AI de transformers.

Pesquisadores de Stanford chamaram os transformers de “modelos de fundação” em um artigo de agosto de 2021 porque os veem impulsionando uma mudança de paradigma na AI. 

> A “escala e o escopo dos modelos de fundação nos últimos anos expandiram nosso entendimento do que é possível”, escreveram.

Transformers estão traduzindo texto e fala quase em tempo real, possibilitando que participantes diversos e com deficiências auditivas participem de reuniões e salas de aula. Eles estão ajudando os pesquisadores a entender as cadeias de genes no DNA e os aminoácidos nas proteínas de maneiras que podem acelerar a criação de medicamentos.

<img src="https://github.com/user-attachments/assets/b0e9ff3e-e0fd-403f-8bd4-363c904fcce0" height="277" align="right">

Os transformers podem detectar tendências e anomalias para evitar fraudes, simplificar a manufatura, fazer recomendações on-line ou melhorar a área da saúde. As pessoas usam transformers toda vez que pesquisam no Google ou no Microsoft Bing.

Uma arquitetura padrão do Transformer, mostrando um codificador à esquerda e um decodificador à direita. Observação: utiliza a convenção pré-LN, que é diferente da convenção pós-LN usada no Transformer original de 2017.

<img width="720" height="730" alt="Screenshot_20241114-132223_Instagram" src="https://github.com/user-attachments/assets/479a06d6-840c-464d-bd75-560a7a69b499" />

Por muitos anos, a modelagem e geração de sequências foi realizada utilizando redes neurais recorrentes simples (RNNs). Um exemplo antigo e bem citado foi a rede de Elman (1990). Em teoria, a informação de um token pode se propagar arbitrariamente ao longo da sequência, mas, na prática, o problema do gradiente evanescente deixa o estado do modelo no final de uma longa frase, sem informações precisas e extraíveis sobre os tokens precedentes.

<img height="777" align="right" src="https://github.com/user-attachments/assets/3da0ab18-a5f6-4021-96de-f12e37725139" />

Um avanço fundamental foi a LSTM (1995),[nota 1] uma RNN que utilizou diversas inovações para superar o problema do gradiente evanescente, permitindo o aprendizado eficiente da modelagem de sequências longas. 

Uma inovação fundamental foi o uso de um mecanismo de atenção que utilizava neurônios que multiplicavam as saídas de outros neurônios, as chamadas unidades multiplicativas. Redes neurais que utilizam unidades multiplicativas foram posteriormente chamadas de redes sigma-pi ou redes de ordem superior. 

A LSTM tornou-se a arquitetura padrão para modelagem de sequências longas até a publicação de Transformers em 2017. No entanto, a LSTM ainda utilizava processamento sequencial, como a maioria das outras RNNs. 

[Nota 2] Especificamente, as RNNs operam um token por vez, do primeiro ao último; elas não podem operar em paralelo em todos os tokens de uma sequência.

Os Transformers modernos superam esse problema, mas, diferentemente das RNNs, requerem um tempo de computação quadrático no tamanho da janela de contexto. O controlador de peso rápido de escala linear (1992) aprende a calcular uma matriz de pesos para processamento posterior, dependendo da entrada. Uma de suas duas redes possui "pesos rápidos" ou "links dinâmicos" (1981). 

Uma rede neural lenta aprende, por gradiente descendente, a gerar chaves e valores para calcular as mudanças de peso da rede neural rápida, que calcula as respostas às consultas. Isso foi posteriormente demonstrado como equivalente ao Transformer linear não normalizado.

A arquitetura Transformers se tornou a base de alguns dos LLMs mais populares, incluindo GPT, Gemini, Claude, DeepSeek e Llama.

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/71298f48-b722-44f9-ac20-3813e4d5061c"></td>
    <td><img src="https://github.com/user-attachments/assets/5437a749-2019-4e2b-a04f-88962b5b114d"></td>
  </tr>
</table>

Funciona assim: Um modelo típico baseado em Transformers possui duas partes principais: o codificador e o decodificador. O codificador lê e interpreta a entrada. O decodificador usa essa interpretação para gerar a saída correta.

1. Na primeira etapa (Incorporação de Entrada), cada palavra é convertida em um número (vetor) que representa seu significado.

2. Em seguida, um padrão chamado Codificação Posicional informa ao modelo a posição de cada palavra na frase. Isso ocorre porque a ordem das palavras é importante em uma frase. Por exemplo, "o gato comeu o peixe" é diferente de "o peixe comeu o gato".

3. A seguir, vem a Atenção Multi-Cabeças, que é o cérebro do codificador. Ela permite que o modelo analise todas as palavras simultaneamente e determine quais palavras estão relacionadas. Na fase de Adição e Normalização, o modelo adiciona o que aprendeu com a atenção de volta à frase.

4. O processo de Feed Forward adiciona profundidade extra à compreensão. O processo geral é repetido várias vezes para que o modelo possa compreender a frase em profundidade.

5. Após a codificação, o decodificador entra em ação. O embedding de saída converte cada palavra da saída esperada em números. Para entender onde cada palavra deve ser inserida, adicionamos a Codificação Posicional.

6. A Atenção Multi-Cabeças Mascarada oculta as palavras futuras, de modo que o modelo preveja apenas uma palavra por vez.

7. A fase de Atenção Multi-Cabeças alinha as partes corretas da entrada com as partes corretas da saída. O decodificador analisa tanto a frase de entrada quanto as palavras que gerou até o momento.

8. O Feed Forward aplica mais processamento para aprimorar a escolha final da palavra. O processo é repetido diversas vezes para refinar os resultados.

9. Assim que o decodificador prevê números para cada palavra, ele os passa por uma Camada Linear para prepará-los para a saída. Essa camada mapeia a saída do decodificador para um grande conjunto de palavras possíveis.

10. Após a Camada Linear gerar pontuações para cada palavra, a camada Softmax converte essas pontuações em probabilidades. A palavra com a maior probabilidade é escolhida como a próxima palavra.

11. Finalmente, é gerada uma frase legível para humanos.

![605764868_1438854998245846_457067546300144168_n](https://github.com/user-attachments/assets/56d67a83-52cf-47dc-8f14-8c0a81bc03d2)
