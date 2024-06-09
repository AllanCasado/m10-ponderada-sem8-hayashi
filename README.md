# Principais Aprendizados
* Trabalho com datasets de pose estimation: Experiência adquirida na manipulação e compreensão de datasets para a tarefa de estimativa de pose, que inclui lidar com os keypoints, pré-processando-os, visualizando-os nas imagens...
* Treinamento de modelos de pose estimation: Construção e treinamento de modelos para identificar e estimar poses de animais em imagens.
* Análise exploratória de imagens: Aplicação de técnicas de análise exploratória em imagens, incluindo histogramas de cores, análise de brilho e saturação média, varição de textura e dimensões das imagens, para entender melhor o dataset e possíveis técnicas de pré processamento para aplicar.

# Limitações
* Modelo não generalizável: O modelo foi desenvolvido especificamente para bovinos e pode não funcionar bem com outros tipos de animais.
* Carga de dados intensiva: Todas as imagens são carregadas de uma vez e, como temos mais de 4k de imagens, pode consumir uma quantidade significativa de recursos de memória e processamento, tornando o sistema lento para grandes datasets.
* Arquitetura simples e perfomance insuficiente: A CNN desenvolvida é bem simples e não alcançou uma boa performance. Possivelmente se usasse arquiteturas mais complexas ou modelos pré-treinados isso seria diferente.
* Variação no número de keypoints: Existe uma inconsistência no número de keypoints por imagem, dentro da categoria de bovinos, o que complica o treinamento e a precisão do modelo.

# Sugestões para Trabalhos Futuros
* Treinamento com outros modelos: Explorar e treinar outros modelos, como o PoseNet do TensorFlow, utilizando técnicas de transfer learning para melhorar a performance.
* Carregamento de dados em batch: Implementar técnicas de carregamento de dados em batch para reduzir o consumo de memória e melhorar a eficiência do treinamento.
* Diversificação do dataset: Ampliar o conjunto de dados para incluir outras categorias de animais, o que aumentaria a capacidade de generalizaçao do modelo.
* Tentar outras técnicas de pré-processamento: Refinar as técnicas de pré-processamento para melhorar a qualidade dos dados de entrada e a eficácia do modelo.
