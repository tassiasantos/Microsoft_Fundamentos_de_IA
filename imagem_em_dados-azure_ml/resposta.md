# Trabalhando com Machine Learning na Prática no Azure ML

![Segmento](https://img.shields.io/badge/Segmento_:-IA-blue?style=flat-square)
![Tecnologias](https://img.shields.io/badge/Tecnologias_:-AzureMachineLearning-lightyellow?style=flat-square) 
![Ano](https://img.shields.io/badge/Ano_:-2025-darkyellow?style=flat-square)

Esta é a minha resposta para o segundo desafio propostro curso Microsoft - Fundamentos de IA oferecido pela DIO.

## Objetivo

Objetivo desse laboratório é praticar a criação de reconhecimento facial, identificação de dados em documentos e também o reconhecimento de elementos em imagens.

### Ferramentas utilizadas:

- Azure: https://portal.vision.cognitive.azure.com
- Serviço da Azure: ``` Azure Vision Studio ```

### Ponto Importante:

 - Caso esteja realizando apenas um prática de estudo, no final excluir tudo que foi construído nesse laboratório. Desta forma, minimiza o risco de ser cobrado algum valor. Lembre-se você está em um ambiente real de produção.


 ### Resumo (Passo-a-passo): Configuração Machine Learning:

# 1 Detectar rostos no Vision Studio

Você pode usar o serviço Azure AI Face com um recurso multisserviço de serviços de IA do Azure. Se ainda não o fez, crie um recurso de serviços de IA do Azure na sua assinatura do Azure.

Em outra guia do navegador, abra o portal do Azure em https://portal.azure.com, entrando com a conta da Microsoft associada à sua assinatura do Azure.

Clique no botão ＋Criar um recurso e pesquise os serviços de IA do Azure. Selecione criar um plano de serviços de IA do Azure. Você será levado a uma página para criar um recurso de serviços de IA do Azure. Configure-o com as seguintes configurações:
Assinatura: sua assinatura do Azure.
Grupo de recursos: selecione ou crie um grupo de recursos com um nome exclusivo.
Região: Selecione a região geográfica mais próxima. Se estiver no leste dos EUA, use “East US 2”.
Nome: Insira um nome exclusivo.
Nível de preços: Padrão S0.
Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo: Selecionado.
Selecione Revisar + criar e depois Criar e aguarde a conclusão da implantação.

# Conecte seu recurso de serviço de IA do Azure ao Vision Studio

Em seguida, conecte o recurso de serviços de IA do Azure provisionado acima ao Vision Studio.

Em outra guia do navegador, navegue até Vision Studio em https://portal.vision.cognitive.azure.com.

Entre com sua conta e certifique-se de usar o mesmo diretório onde você criou seu recurso de serviços de IA do Azure.

Na página inicial do Vision Studio, selecione Visualizar todos os recursos no título Introdução ao Vision.

Na página Selecione um recurso para trabalhar, passe o cursor do mouse sobre o recurso que você criou acima na lista e marque a caixa à esquerda do nome do recurso e selecione Selecionar como recurso padrão.

Feche a página de configurações selecionando o “x” no canto superior direito da tela.

# Detecte rostos no Vision Studio

Num navegador web, navegue até Vision Studio em https://portal.vision.cognitive.azure.com.

Na página inicial Introdução ao Vision, selecione a guia Face e, em seguida, selecione o bloco Detectar rostos em uma imagem.

No subtítulo Experimente, reconheça a política de uso de recursos lendo e marcando a caixa.

Selecione cada uma das imagens de amostra e observe os dados de detecção facial retornados.

Agora vamos tentar com algumas de nossas próprias imagens. Selecione https://aka.ms/mslearn-detect-faces para baixar detect-faces.zip. Em seguida, abra a pasta no seu computador.

Localize o arquivo chamado store-camera-1.jpg; que contém a seguinte imagem:

Faça upload de store-camera-1.jpg e revise os detalhes de detecção de rosto retornados.

Localize o arquivo chamado store-camera-2.jpg; que contém a seguinte imagem:


![Captura de tela 2025-02-02 033944](https://github.com/user-attachments/assets/e26012b5-3373-445d-b907-5951fe960200)


![Captura de tela 2025-02-02 040014](https://github.com/user-attachments/assets/e1e12701-9324-4a05-8835-7c3a08918fab)


![Captura de tela 2025-02-02 040031](https://github.com/user-attachments/assets/51a88178-8bd3-4df9-8cf8-981afe0e9283)


![Captura de tela 2025-02-02 040153](https://github.com/user-attachments/assets/f23034ae-218d-41a2-adf6-ac4ea843bc1b)


![Captura de tela 2025-02-02 040441](https://github.com/user-attachments/assets/51cd1b00-6fe3-4922-8983-ebe24c346ed1)


![Captura de tela 2025-02-02 041250](https://github.com/user-attachments/assets/2a655a1b-d9e3-4505-be4a-dd2dcde4b631)



## 2 Ler texto no Vision Studio

# Extraia texto de imagens no Vision Studio

Num navegador web, navegue até Vision Studio em https://portal.vision.cognitive.azure.com.

Na página inicial Introdução ao Vision, selecione Reconhecimento óptico de caracteres e, em seguida, o bloco Extrair texto de imagens.

No subtítulo Experimente, reconheça a política de uso de recursos lendo e marcando a caixa.

Selecione https://aka.ms/mslearn-ocr-images para baixar ocr-images.zip. Em seguida, abra a pasta.

No portal, selecione Procurar um arquivo e navegue até a pasta em seu computador onde você baixou ocr-images.zip. Selecione advert.jpg e selecione Abrir.

Agora revise o que é retornado:
Nos atributos detectados, qualquer texto encontrado na imagem é organizado em uma estrutura hierárquica de regiões, linhas e palavras.
Na imagem, a localização do texto é indicada por uma caixa delimitadora, conforme mostrado aqui:


![Captura de tela 2025-02-02 041547](https://github.com/user-attachments/assets/995ad840-42d6-4a81-93e8-e08d4c38b279)


![Captura de tela 2025-02-02 042000](https://github.com/user-attachments/assets/0dfd77a7-b368-407f-b3c8-15cef7baa83e)


## 3 Analise imagens no Vision Studio

# Gerar legendas para uma imagem

Agora você está pronto para usar o Vision Studio para analisar imagens tiradas por uma câmera na loja Northwind Traders.

Vejamos a funcionalidade de legenda de imagens do Azure AI Vision. As legendas das imagens estão disponíveis por meio dos recursos Legenda e Legendas densas.

Em um navegador da web, navegue até Vision Studio.

Na página inicial Introdução ao Vision, selecione a guia Análise de imagem e, em seguida, selecione o bloco Adicionar legendas às imagens.

No subtítulo Experimente, reconheça a política de uso de recursos lendo e marcando a caixa.

Selecione https://aka.ms/mslearn-images-for-análise para baixar image-análise.zip. Abra a pasta no seu computador e localize o arquivo chamado store-camera-1.jpg; que contém a seguinte imagem:

Carregue a imagem store-camera-1.jpg arrastando-a para a caixa Arrastar e soltar arquivos aqui ou navegando até ela em seu sistema de arquivos.

Observe o texto da legenda gerado, visível no painel Atributos detectados à direita da imagem.

A funcionalidade Caption fornece uma frase em inglês única e legível que descreve o conteúdo da imagem.

Em seguida, use a mesma imagem para realizar legendas densas. Retorne à página inicial do Vision Studio e, como fez antes, selecione a guia Análise de imagem e, em seguida, selecione o bloco Legenda densa.

O recurso Dense Captions difere do recurso Caption porque fornece várias legendas legíveis para uma imagem, uma descrevendo o conteúdo da imagem e outras, cada uma cobrindo os objetos essenciais detectados na imagem. Cada objeto detectado inclui uma caixa delimitadora, que define as coordenadas dos pixels na imagem associada ao objeto.

Passe o mouse sobre uma das legendas na lista de atributos detectados e observe o que acontece na imagem.

![Captura de tela 2025-02-02 042118](https://github.com/user-attachments/assets/4fe1c052-de01-480a-a094-a41240cc5026)


![Captura de tela 2025-02-02 042742](https://github.com/user-attachments/assets/91301d91-0b85-4842-ac99-21b87d710d89)


