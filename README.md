## Projeto de Engenharia de Dados - Streaming de Dados

# Caminhões SA  
<div align="left">
<img src="https://github.com/Lucas-Sobreira/Azure_Streaming_Caminhoes_SA/blob/main/imgs/logo.png" width="200" height="50"/>
</div>

## Contexto e objetivos do projeto
<p align="justify">
A Caminhões SA, uma empresa especializada em transporte de alimentos refrigerados, está embarcando em um projeto estratégico de monitoramento de temperatura dentro de seus caminhões frigoríficos. A empresa reconhece a importância crítica de manter as temperaturas dentro dos caminhões em níveis ideais para garantir a qualidade e a segurança dos produtos transportados. Com o objetivo de aprimorar seu processo de monitoramento, a Caminhões SA está investindo em um sistema de engenharia de dados que permitirá a coleta e análise em tempo real dos dados de temperatura.
</p>

## Descrição do projeto
<p align="justify">
O objetivo deste projeto é criar um pipeline de dados para a ingestão em tempo real de informações de sensores de temperatura instalados em caminhões frigoríficos da empresa Caminhões SA. Esses sensores monitoram constantemente a temperatura dentro dos caminhões, garantindo a integridade dos alimentos refrigerados durante o transporte. Os dados coletados pelos sensores são transmitidos em tempo real para um sistema central de análise.

Os <b>dados são fictícios</b>, sendo originados de um Job em Python. 
</p>

### <ins>Requisito Funcional</ins>

1) Criar um EventHub e o DataLake;
2) Testar o envio das informações para o EventHub e para o DataLake;
3) Criar o Azure Stream Analytics para analisar os dados do EventHub;
4) Construir o App do Caminhoes SA;
5) Testar a solução completa e conectar ao Power BI;

## Arquitetura

- <b><ins>Ideia de arquitetura</ins>:</b>

<div align="center">
<!-- <img src="https://github.com/Lucas-Sobreira/Azure_Streaming_Caminhoes_SA/blob/main/imgs/Arquitetura_EventHub.png" width="800" height="450"/> -->
<img src="https://github.com/Lucas-Sobreira/Azure_Streaming_Caminhoes_SA/blob/main/imgs/Arquitetura_EventHub.png" width="650" height="350"/>
</div>

<br>

- <b><ins>Arquitetura do projeto</ins>:</b>

<div align="center">
<img src="https://github.com/Lucas-Sobreira/Azure_Streaming_Caminhoes_SA/blob/main/imgs/arquitetura_projeto.png" width="650" height="230"/>
</div>

<br>

<p align="justify">
Para a implementação deste projeto, utilizamos uma arquitetura baseada na plataforma Azure da Microsoft, aproveitando as seguintes tecnologias:
</p>

- <p align="justify"> <b>Azure Event Hubs:</b> O Azure Event Hubs é o ponto de entrada para os dados provenientes dos sensores dos caminhões. Este serviço atua como um hub de eventos altamente escalável, permitindo a ingestão, processamento e armazenamento de informações em tempo real. Os dados são recebidos aqui a partir dos sensores e encaminhados para a próxima etapa do pipeline.</p>

- <p align="justify"> <b> Azure Stream Analytics:</b> O Azure Stream Analytics é responsável por realizar análises em tempo real nos dados recebidos. Ele processa milhões de eventos de streaming por segundo, permitindo que a equipe de monitoramento da Caminhões SA identifique imediatamente qualquer desvio nas temperaturas dos caminhões frigoríficos. Caso sejam detectadas anomalias, ações corretivas podem ser acionadas em tempo hábil.</p>

- <p align="justify"> <b>Azure Data Lake Storage Gen2:</b> Os dados são armazenados no Azure Data Lake Storage Gen2. Este sistema de arquivos corporativo é otimizado para análises de big data, suportando uma variedade de cargas de trabalho, incluindo processamento com Hadoop, Spark e outras ferramentas. O Data Lake armazena um histórico completo dos dados de temperatura, o que é valioso para análises retrospectivas e tendências ao longo do tempo.</p>

## Conclusão e próximos passos
<p align="justify">
Este projeto de engenharia de dados de streaming atende aos objetivos estratégicos da Caminhões SA, proporcionando à empresa uma maneira eficiente de monitorar e registrar as temperaturas dentro de seus caminhões frigoríficos em tempo real. A capacidade de resposta imediata a qualquer anomalia nas temperaturas é crucial para garantir a qualidade e segurança dos produtos transportados. Este sistema também permite análises retrospectivas para melhorar ainda mais as operações da empresa.</p>

<p align="justify">Para próximos passos do projeto, pode ser uma melhora no Dashboard realizado até o momento, inclusive utilizando as informação de <b>geolocalização</b> que não foram utilizadas por motivos de <b>limitação de assinatura</b>.</p>

<div align="center">
<img src="https://github.com/Lucas-Sobreira/Azure_Streaming_Caminhoes_SA/blob/main/imgs/relatorio.png" width="1100" height="500"/>
</div>
