# Projeto de Data Science - Acompanhamento das Eleições

## Descrição do Projeto
Este projeto foi desenvolvido para acompanhar as eleições durante um período específico utilizando dados de redes sociais, principalmente do Twitter. Foi meu primeiro projeto focado em Data Science, realizado antes de iniciar meu curso de especialização. Como resultado, pode conter algumas redundâncias e abordagens que na época ainda não sabia como otimizar.

O principal objetivo foi coletar, tratar e analisar os dados de forma a prever tendências e opiniões durante o período eleitoral.

## Tecnologias Utilizadas
- **SNScrape**: Utilizado para coleta de dados do Twitter.
- **NLTK** e **Scikit-learn**: Utilizados para tratamento e classificação de dados.
- **Naive Bayes**: Algoritmo de aprendizado de máquina escolhido para a tarefa de classificação.
- **PowerBI**: Ferramenta para visualização dos dados e criação do dashboard.

## Coleta de Dados
A coleta dos dados foi realizada utilizando a biblioteca [SNScrape](https://github.com/JustAnotherArchivist/snscrape), que permite acessar dados de redes sociais. O foco foi em tweets relevantes para o período eleitoral, coletando informações como:
- Texto do tweet
- Data de publicação
- Usuário

Os dados foram coletados de forma contínua durante o período analisado e armazenados em um formato adequado para processamento.

## Tratamento de Dados
Para o pré-processamento dos dados, as seguintes técnicas foram aplicadas:
1. **Remoção de stop words**: Palavras comuns como "de", "para", "o", etc., foram removidas para reduzir ruído nos dados.
2. **Stemming**: Redução das palavras ao seu radical para normalizar termos similares.
3. **Vetorização**: Transformação dos textos em dados numéricos para alimentar o modelo de aprendizado de máquina.

## Modelos de Predição
A classificação foi realizada utilizando o algoritmo **Naive Bayes**, implementado com a ajuda das bibliotecas **Sklearn** e **NLTK**. Para treinar o modelo, utilizei um conjunto de dados previamente classificado para atribuir valor às amostras coletadas.

## Armazenamento de Resultados
Os resultados foram armazenados em um arquivo Excel, facilitando a manipulação posterior e a visualização no dashboard.

## Visualização dos Dados
Um dashboard interativo foi construído utilizando **PowerBI**, onde é possível visualizar as principais métricas e análises geradas a partir dos dados coletados e processados. O dashboard está localizado no diretório `Dashboard` e pode ser acessado como o segundo arquivo do diretório.

## Diretórios do Projeto
- **/data**: Contém os dados brutos e processados.
- **/models**: Scripts relacionados à construção e treinamento do modelo.
- **/dashboard**: Arquivo PowerBI com as visualizações criadas.

## Considerações Finais
Este projeto foi meu primeiro passo na área de Data Science, e embora apresente algumas limitações e possíveis redundâncias, ele serviu como uma base sólida para projetos futuros. Sugestões e melhorias são bem-vindas!

