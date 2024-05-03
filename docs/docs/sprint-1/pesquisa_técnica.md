---
label: "Pesquisa Técnica"
---

# Pesquisa Técnica

## Geração aumentada de recuperação (RAG)
Retrieval-Augmented Generation (RAG) é o processo de otimizar a saída de um grande modelo de linguagem, de forma que ele faça referência a uma base de conhecimento confiável fora das suas fontes de dados de treinamento antes de gerar uma resposta. 

Grandes modelos de linguagem (LLMs) são treinados em grandes volumes de dados e usam bilhões de parâmetros para gerar resultados originais para tarefas como responder a perguntas, traduzir idiomas e concluir frases.

A RAG estende os já poderosos recursos dos LLMs para domínios específicos ou para a base de conhecimento interna de uma organização sem a necessidade de treinar novamento o modelo. 

O LLM é uma tecnologia fundamental utilizada pela inteligência artificial alimenta chatbots inteligentes e outras aplicações de processamento de linguagem natural (PLN). 

Os LLMs enfrentam uma série de desafios atualmente, como os seguintes:

1. Fornecer informações falsas quando não possuem uma resposta adequada.
2. Oferecer informações desatualizadas ou genéricas quando os usuários solicitam respostas específicas e atualizadas.
3. Gerar respostas baseadas em fontes não confiáveis.
4. Criar respostas imprecisas devido à confusão terminológica, quando diferentes fontes de treinamento utilizam a mesma terminologia para descrever conceitos distintos.

Dessa maneira, os maiores benefícios da geração aumentada de recuperação, podem ser:

1. Implementação econômica: Geralmente, a criação de chatbots começa com a utilização de um modelo de base. Os modelos de base (FMs) são modelos de ML treinados em um amplo espectro de dados generalizados e não rotulados. Os custos computacionais e financeiros que são necessários para atualizar os FMs com informações específicas da organização ou do domínio são altíssimos. RAG oferece uma abordagem para incorporar novos dados no LLM que é mais viável economicamente. Isso faz com que a tecnologia de inteligência artificial generativa (IA generativa) seja mais acessível e aplicável em grande escala.
2. Informações atualizadas: Mesmo que as fontes de dados de treinamento originais de um LLM sejam adequadas às suas necessidades, a manutenção da sua relevância continua sendo desafiadora. O RAG possibilita que desenvolvedores forneçam dados de pesquisa, estatísticas ou notícias mais recentes diretamente aos modelos generativos. Através dessa abordagem, é possível conectar o LLM a feeds de mídia social ao vivo, sites de notícias ou outras fontes de informações atualizadas frequentemente de maneira direta. O LLM então pode fornecer as informações mais recentes aos usuários.
3. Maior confiança de usuários: Com a tecnologia RAG, o LLM pode apresentar informações precisas com atribuição de fontes. O resultado pode conter citações ou referências às fontes utilizadas. Os usuários também podem consultar os documentos de origem, caso precisem de mais esclarecimentos ou detalhes. Isso pode aumentar a confiança e credibilidade na sua solução de IA generativa.
4. Maior controle na etapa de desenvolvimento: A tecnologia RAG também permite que a equipe de desenvolvimento teste e aprimore os recursos de conversação ou chat de forma mais eficiente. É possível gerenciar e modificar as fontes de informação do LLM para adequá-las a necessidades mutáveis ou para uso multifuncional. A equipe de desenvolvimento tem a capacidade de limitar o acesso a informações sensíveis de acordo com níveis de autorização, assegurando que o LLM produza respostas adequadas. Além disso, podem intervir e realizar correções caso se o LLM referenciar fontes de informação incorretas para perguntas específicas. As organizações podem adotar a tecnologia de IA generativa com maior segurança para um leque mais vasto de aplicações.

### Como funciona a geração aumentada de recuperação?
Na ausência da RAG, o LLM depende da entrada do usuário para criar uma resposta de acordo com as informações de treinamento ou de base. Com a implementação da RAG, é introduzido um componente de recuperação de informações que utiliza a entrada do usuário para extrair informações de uma nova fonte de dados primeiro. A consulta do usuário e as informações relevantes são fornecidas ao LLM. O LLM usa esse novo conhecimento e seus dados de treinamento para criar respostas mais adaptadas. As seções a seguir fornecem uma visão geral do processo.

Criação de dados externos
Os novos dados, que não fazem parte do conjunto de dados de treinamento original do LLM, são chamados de dados externos. Esses dados podem ser obtidos de múltiplas fontes, como APIs, bancos de dados ou repositórios de documentos. Os dados podem existir em vários formatos, como arquivos, registros de banco de dados ou texto longo. Outra técnica de IA, chamada de incorporação de modelos de linguagem, converte os dados em representações numéricas e os armazena em um banco de dados de vetores. Esse processo cria uma biblioteca de conhecimento que os modelos de IA generativa podem compreender.

Recuperação de informações relevantes
A próxima etapa é realizar uma pesquisa de relevância. A consulta do usuário é convertida em uma representação vetorial e combinada com os bancos de dados de vetores. Por exemplo, considere um chatbot inteligente que responde perguntas relacionadas a recursos humanos para uma organização. Se um funcionário pesquisar "Quantas férias anuais eu tenho direito?", o sistema recuperará os documentos da política de férias anuais junto com o registro de férias anteriores do funcionário. Esses documentos específicos serão fornecidos porque são altamente relevantes para a consulta em questão. A relevância foi calculada e estabelecida através de cálculos e representações vetoriais matemáticas.

Enriquecimento de prompts fornecidos ao LLM
Em seguida, o modelo RAG enriquece a entrada do usuário, também chamada de prompt, adicionando os dados recuperados que são relevantes ao contexto. Esta etapa usa técnicas de engenharia de prompts para se comunicar de forma eficaz com o LLM. Com um prompt enriquecido, os grandes modelos de linguagem podem gerar respostas mais contextualizadas às consultas dos usuários.

Atualização de dados externos
Mas daí surge outra questão: e se os dados externos ficarem obsoletos? Para manter a contemporaneidade das informações, basta atualizar os documentos de forma assíncrona e atualizar a representação incorporada dos documentos. Isso pode ser feito através de processos automatizados em tempo real ou de processamento em lotes periódicos. Esse é um desafio comum na análise de dados, onde diversas metodologias provenientes da ciência de dados para gestão de mudanças são aplicáveis.

### Como RAG funciona para personalizar os LLMs?
Sem o uso de RAG, o LLM depende da entrada do usuário para criar uma resposta de acordo com os dados que recebeu durante o treinamento. Assim, como o uso de RAG, é introduzido um componente de recuperação de informações que utiliza a entrada do usuário para extrair informações de uma nova fonte de dados primeiro. A consulta do usuário e as informações relevantes são fornecidas ao LLM. O LLM usa esse novo conhecimento e seus dados de treinamento para criar respostas mais adaptadas. As seções a seguir fornecem uma visão geral do processo.

**Criação de dados externos**
Os novos  dados, que não fazem parte do conjunto de dados de treinamento original do LLM, são chamados de dados externos. Esses dados podem ser obtidos de múltiplas fontes, como APIs, bancos de dados ou repositórios de documentos.

Os dados podem existir em vários formatos, como arquivos, registros de banco de dados ou texto longo. Outra técnica de IA, chamada de incorporação de modelos de linguagem (ou apenas criação de embeddings), converte os dados em representações numéricas e os armazena em um banco de dados de vetores. Esse processo cria uma biblioteca de conhecimento que os modelos de IA Generativa podem compreender.

**Recuperação de informações relevantes**
A próxima etapa é realizar uma pesquisa de relevância. A consulta do usuário é convertida em uma representação vetorial e combinada com os bancos de dados de vetores.

Por exemplo, considere um chatbot inteligente que responde perguntas relacionadas a recursos humanos para uma organização. Se um funcionário pesquisar “Quantas férias anuais eu tenho direito?”, o sistema recuperará os documentos da política de férias anuais junto com o registro de férias anteriores do funcionário. Esses documentos específicos serão fornecidos porque são altamente relevantes para a consulta em questão. A relevância foi calculada e estabelecida através de cálculos e representações vetoriais matemáticas.

**Enriquecimento de prompts fornecidos ao LLM**
Em seguida, o modelo RAG enriquece a entrada do usuário, também chamada de prompt, adicionando os dados recuperados que são relevantes ao contexto. Esta etapa usa técnicas de engenharia de prompts para se comunicar de forma eficaz com o LLM. Com um prompt enriquecido, os grandes modelos de linguagem podem gerar respostas mais contextualizadas às consultas dos usuários. 

**Atualização de dados externos**
Mas daí surge outra questão: e se os dados externos ficarem obsoletos? Para manter a contemporaneidade das informações, basta atualizar os documentos de forma assíncrona e atualizar a representação incorporada dos documentos. Isso pode ser feito através de processos automatizados em tempo real ou de processamento em lotes periódicos. Esse é um desafio comum na análise de dados, onde diversas metodologias provenientes da Ciência de Dados para gestão de mudanças são aplicáveis.

Resumindo, podemos entender o grande modelo de linguagem (LLM) como um funcionário recém-contratado que opta por ignorar as notícias atuais, mas mesmo assim responde a todas as perguntas com total convicção. Contudo, essa abordagem pode impactar negativamente a confiança dos usuários, o que não é desejável, obviamente!

A abordagem RAG pode ser usada para solucionar alguns desses desafios. Ela direciona o LLM a recuperar dados relevantes, provenientes de fontes de conhecimento confiáveis e previamente definidas. Dessa maneira, as organizações ganham mais controle sobre o texto gerado e os usuários recebem respostas melhores do LLM.

Para uma empresa (e provavelmente para qualquer pessoa) usar apenas o LLM é arriscado, pois a chance de respostas erradas é muito grande. O uso de RAG personaliza um LLM com fontes de dados confiáveis, tornando seu uso no dia a dia muito mais seguro.

## Conclusão
Em resumo, a RAG oferece uma abordagem poderosa para superar os desafios enfrentados pelos LLMs, permitindo a personalização do modelo com fontes de dados confiáveis. Isso não só aumenta a confiança dos usuários, mas também torna o uso diário de LLMs mais seguro e eficaz para organizações e usuários em geral.

# Bibliografia
https://aws.amazon.com/pt/what-is/retrieval-augmented-generation/
https://blog.dsacademy.com.br/como-rag-retrieval-augmented-generation-funciona-para-personalizar-os-llms/
https://medium.com/data-hackers/construindo-aplica%C3%A7%C3%B5es-personalizadas-com-llm-atrav%C3%A9s-de-rag-retrieve-augmented-generation-6f3a3df7b6de
https://www.oracle.com/br/artificial-intelligence/generative-ai/retrieval-augmented-generation-rag/
https://learn.microsoft.com/pt-br/azure/search/retrieval-augmented-generation-overview 
