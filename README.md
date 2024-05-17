# Pipeline-GCP
## Pipeline de Dados com Google Cloud Platform


Problema:	Saber quantas empresas CNPJ tem no Brasil, por região, e classificá-las 
 Solução:	Construir um pipeline para extração, transformação e carga da base de dados abertos de CNPJs do Governo Federal.

	O Download manual da base de dados do portal de dados aberto é lento então, para mitigar esse problema, coloquei toda a solução em cloud para evitar gargalos nas máquinas locais.
	Para reduzir os custos de operações em cloud, criei um processo de atualização mensal, em sincronia com as atualizações da base de dados aberto que também é mensal.

	O propósito desse artigo, que também serve de documentação do processo, não visa esgotar o assunto, dado que tem formas mais eficientes de solucionar esse deasafio, mas também
	servir de estudo de caso, e consulta para estudantes e iniciantes em engenharia de dados, além de provocar a criatividade nos mais avançados para melhoria do processo.

	Por quê Google Cloud? 🤔
	Os fatores que pesaram na decisão foram, a facilidade de uso e a redução de custos. O GCP é intuitivo, ambiente codeless com bastante funções visuais, ao passo que também
	temos a oportunidade de desenvolver nosso código e implementar na solução. Além disso, o Google disponibiliza US$300 em créditos para novos usuários.

	Serviços utilizados:
		🖥 Compute Engine (VM para execução dos scripts)
		🗄 Cloud Storage (Armazenamento dos dados)
		🗃 Google BigQuery (Análise dos dados)
		📊 Looker Studio (Dashboard com análises)
