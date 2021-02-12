# TCC - Virtualização Open-Source Para Aplicações Focadas em Infrastrutura Computacional


Este Trabalho tem como foco a virtualização de recursos computacionais.
A virtualização onde se pode atingir grande poder computacional voltado 
a disponibilidade e de escalonamento de serviços, armazenamento, para prover 
grandes estruturas seja de sistema ou ate mesmo de hardware com isso veio a 
computação de alto desempenho com aplicações desses serviços focado em máquinas virtuais.

Disponibilidade:
Para essas aplicações tenhamos um serviço ininterrupto como a proposta de servidores
web e servidores dns, a disponilidade atrelado a virtualização permite maior flexibilidade e prover de mais recursos por estar em ambiente de máquinas virtuais.

Escalonamento:
Junto as máquinas de virtualização a troca de contexto muito uitlizado por estrutura 
computacional  provendo de mais recursos para um aumento de demandas, essas orquestrações muitas das vezes estão em provisionamnto em data-centers onde muitas máquinas virtuais.


Manutenção:
Para fazer alguma manutenção levando em consideração que a camada de virtualizaçao o qual não atingi ao sistema nativo uma vez que a camada de virtualiza permite que remove, 
cria, backup dos sistemas das VMs , e se houver a necessidade de escalonar aplicações também é possível, pensando nisso para que a dispobinilidade funcione altera apenas a
camada de virtualização onde estão os sistema virtuais.

Armazenamento:
Todas parte de storage ficam disposto para cada VMs onde cada um deles tem seu próprio armazenamento, cada sistema então consiste em ter seu proprio storage para o trabalho isolado de cada um deles. 

Processamento:
Contudo a virtualização de recurso computacional uma das principais funções é prove mais processamento para a orquestração de máquinas virtuais, 
o intuito dessa aplicação tem como requisito obter maior processanamento ganhando performace em sistema ao qual venha desempenhar suas funções. 
Ao escalonar o processamento permitir analisar e processar grandes quantidades de dados, este trabalho seria mais utilizado para computação de alto desempenho onde divide o processamentos em vários computadores virtuais afim de se obter maior vantagem computacional

Falha de serviço:
Como obtenção da camadad de virtualizaçao permitir reduzir a falhas de serviços adotado para os servidores, 
isso é permitido atravez do método de virtualizar e com a disponibilidade de recursos virtuais, garantindo mais
redundâncias e previnir que tenha falhas de algum serviço criando outras instâncias das máquinas virtuais.

Server Web
Para que tenhamos um ambiente de avaliação, podemos equiparar os mesmo tipos de serviços em nuvem utilizado, pensando nisso essa implementação tem como objetivo analisar
a disponilidade de serviços por contar um servidor web onde esta fazendo parte em VMs primário e secundário, assim tenhamos um dispobinilidade e reduncia.
	Docker	
Utilizado a plataforma para obtenção e prover um container com a aplicaçao web.
 	Apache
O Apache cria uma imagen desse container com os arquivos da aplicação.

Bind9
	Barkley internet domain, utilziado para resolver o domínio local dos servidores Web
  
FirewallD
Utilizado apenas para liberar os serviços HTTP e portas os quais os serviços e servidores necessitam para fazer o compartilhamento em rede das aplicação em questão,
domínio implementado local, ao subir oserviço da aplicação docker em container onde dispobiliza um um serviço de virtualição com o apache.

Server DNS:
A implementação do DNS nessa avaliação, permiti que resolva nomes de domínios agora do servidor web previamente
estabelecido e configurado para que publique na rede e que os recursos e aplicações web fica acessível na rede, não tem muita distinção 
de fazer os servidores virtuais web para os servidores DNS, porém para o servidro DNS utiliza o nameD onde o qual é o serviço nativo do CentOS assim 
como o bind levanta um serviço de domínio sendo que no servidor DNS agora resolve para a rede.


Aplicação Web e comportamento das páginas
Então temos a aplicação ao servidor onde ele pode ser um no de algum cluster previamente, 
aqui poderia compor uma parte de micro-servidor ou outros tipos de servidores como, banco dados, FTP, servidor de email,
estando interligado começa a prover de recursos para rede, atraves do hyper-v, consequentemente temos os servidores virtuais o qual pode conter container de aplicação 
variadas e aplicação de multilinguagens, para o container o docker foi implementado com intuito de orquestrar e definir um serviço web.




