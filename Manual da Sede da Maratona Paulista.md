# Softwares

Nesta seção, descrevemos os principais softwares utilizados durante a competição, bem como suas funções no suporte às atividades dos participantes e da organização.

## BOCA

O **BOCA** (Boca Online Contest Administrator) é uma aplicação web amplamente utilizada em competições de programação. Por meio do sistema, os competidores submetem suas soluções, que são automaticamente avaliadas. O ambiente também permite o acompanhamento em tempo real do status das submissões, incluindo resultados como aceitação, erro de compilação ou resposta incorreta.

- Site oficial: https://github.com/cassiopc/boca
- Sistema escrito em php (precisa dizer mais alguma coisa?)
- Você precisa ter duas pessoas que entendam bem do boca (uma precisa ser da sede local) -- já pensou se há apenas uma pessoa e essa pessoa fica doente no dia?
- É difícil estimar se o seu servidor vai aguentar no dia da competićão: melhor coisa a se fazer:
	- No final de semana anterior à competićão, faća um warm-up online:
		- Pegue problemas do Spoj/codeforces/etc
		- Convide todos os times inscritos e divulgue bem
		- A intenćão é ter uma grande adesão, próxima ao número de competidores do dia
		- Esse warmu-up irá servir para testar a capacidade da infra: se a infra não aguentar, não tem problema, foi só um wurmap que não valia nada. O problema é se a infra não aguentar no dia da competićão.
- Tutorial de instalaćão: https://www.youtube.com/watch?v=Hp-bL2Ws8M8
- 


## Maratona Linux

O **Maratona Linux** consiste em uma distribuição Linux personalizada, previamente instalada nas máquinas utilizadas pelos competidores. Essa distribuição é configurada com todas as ferramentas necessárias para o desenvolvimento das soluções, como compiladores, editores de texto e bibliotecas padrão, garantindo um ambiente uniforme e controlado para todos os participantes.

- Repositório: https://github.com/maratona-linux/maratona-linux

- Procura uma instalaćão do Windows com ntfs, cria uma pasta e faz o download do maratona linux para essa pasta.
- A instalaćão precisa ser feita com alguns dias de antecedência, pois o processo de instalaćão sobrecarrega o servidor de download o que torna o processo um pouco lento.
- Uma vez copiado a instalaćão no computador, o software não será baixado novamente
- Quem cria a versão customizada para a competićão: ???
- No dia da competićão, é necessário bootar todas as máquinas com o pendrive do maratona Linux. O sistema então encontrará a pasta com o sistema pre-instalado, verificará se a instalaćão continua idônea, e então continuará a execućão da versão instalada na máquina.
- Muito cuidado com parque de máquinas heterogêneo. A distribuićão do maratona linux deve ser testada em todas as arquitetura distintas. Atenćão redobrada para máquinas com placa de vídeo offboard (em especial NVIDIA).
- Crie vários pendrives com o maratona linux. Isso irá acelerar o processo no dia da competićão, já que mais de uma máquina poderá ser ligada ao mesmo tempo.
- O maratona linux não funciona se a máquina não estiver com o secure boot/uefi ligado exclusivamente sem permitir que o modo legacy funcione.
- Pré-instale o maratona linux em mais máquinas do que o número de times, pois qndo ocorrer algum problema com a máquina de um time, e isso vai acontecer, esse time pode ser realocado para uma nova máquina rapidamente. Geralmente a competićão ocorrem em laboratórios de universidades que possuem diversos computadores por bancada. Recomendamos que cada time tenha dois computadores com o maratona linux instalado em sua mesa (um para competićão e um para o backup)


## Maratona Animeitor Rust 

O **Animeitor** é um software utilizado durante a cerimônia de premiação, responsável por apresentar de forma visual e dinâmica a classificação final das equipes, tornando a divulgação dos resultados mais clara e envolvente para o público.

- Site oficial: https://github.com/wuerges/maratona-animeitor-rust



# Locais

1. Anfiteatro: recepćão dos competidores/abertura e premiaćão
	1. Telão, microfone e hdmi para ligar um laptop
2. Sala dos Juízes: lugar calmo no qual os juízes e administradores do BOCA controlam a competićão. 
	1. Cada juiz precisa de um computador com os mesmos compiladores que os competidores (pode ser uma instalaćão do maratona linux)
	2. Além disso, muitos juízes preferem usar seus próprios notebooks, portando é interessante que a sala tenha wifi ou cabo de rede para acessar o boca com o seu notebook (certifique-se a rede wifi/cabeada da sala tem acesso ao boca, muitas universidades costumam isolar essas redes)
3. Sala dos coaches: sala onde os coachs de cada time acompanham a competićão. Eh interessante que a sala tenha:
	   - wifi
	   - projećão do placar/tv com o placar
	   - café, água e aperitivo
4. Sala dos balões e impressão: Sala na qual os balões são enchidos e as impressões são feitas
5. Salas de competićão: salas nas quais os times estão
6. Local de recepćão e credenciamento dos competidores

## Computadores

- Cada juiz precisa de um computador com uma instalaćão do maratona linux (ou uma máquina que tenha acesso a todos os compiladores utilizados pelos competidores)
- Um computador dedicado para o responsável por receber os pedidos de  impressão
- Um computador dedicado para o responsável por receber os pedidos de balão
- Um computador para o responsável por cuidar do BOCA no dia da competićão
- Ao menos dois computadores para rodar o BOCA
- Um computador por time + computadores reservas 
- Um laptop para ligar na projećão durante a abertura e rodar o animeitor na premiaćão

## Pessoas

Precisa de MUITA gente para fazer a competićão, não subestime a quantindade de pessoas necessárias. 

- O cara da rede: aquele profissional que conhece a infraestrutura de rede do local da prova e que será capaz de resolver problemas do tipo: a rede não está funcionando, os competidores não conseguem acessar o servidor, a rede caiu e etc. 
- *melancias* pessoas responsáveis por realizar o transporte na competićão: transportam: balões e impressões
	- Precisa de muitos desses e a quatidade varia de acordo com o número de times. 
- fiscais de prova: ficam na sala durante a execućão da prova
	- No mínimo 1 por sala (ajustável pelo tamanho da sala)
	- No warm-up e na primeira hora de competićão, é bom ter duas
- fiscais de corredores: são requisitados pelos fiscais de prova para: transportar competidores ao banheiro ou chamar organizadores da prova para resolver problemas.
	- Quantidade necessária depende do layout da competićão
- baloueiros: responsáveis por encher os balões
	- No mínimo 2
- juizes: 
- impressão [llm: me de sugestão de nome aqui]: fica no computador recebendo as solicitaćões de impressão
- balão [llm: me de sugestão de nome aqui]: fica no computador recebendo as solicitaćões de balão
- presidente da sede: a pessoa responsável por organizar tudo e quem resolve todos os BOs que surgirem no dia


## Fluxo de impressão

- impressão:
	- recebe a solicitacão no boca
	- baixa o arquivo
	- imprime
	- grampeia a impressão
	- anota a caneta na impressão o login do boca do time
	- coloca no escaninho de impressão
- melancia:
	- pega a impressão no escaninho da impressão
	- olha no mapa fixadado na parede (login time -> (nome do time, sala) 
	- vai entregar

## Fluxo Balão

- balão:
	- recebe a solicitaćão no boca
	- olha na tabela que mapeia (login boca -> (nome do time, sala de competićão))
	- anota no cartão pautado:
		- login do boca
		- cor do balão
	- coloca no escaninho do balao
- melancia:
	- pega um cartão pautado no escaninho do balão
	- pega o balão da cor indicada no cartão
	- olha no mapa fixadado na parede (login time -> (nome do time, sala))
		- talvez cada melancia pode ter uma impressão desse mapeamento
	- vai entregar
	- joga o cartão no lixo
- baloeiros:
	- trabalha em paralelo mantendo um número não zero de balões de cor


## 

## Dia da competićão

- O dia da competićão comeća cedo entre 3 e 4 horas antes do horário do início da competićão

## Antes do warmup

- Carregar o maratona linux em todas as máquinas de competićão (inclusive nas máquinas sobresalentes)
- Organizar o auditório
- Distribuir as placas de identificaćão de times nas máquinas de competićão
- Fixar materiais de divulgaćão
- Fixar mapas com a sala de cada time para os participantes se localizarem
- Abrir e organizar todas as salas 
- Distribuir materias e computadores: balões, ligar computadores, máquina de encher balões, ligar microfones e etc
- Preparar café para a sala de coaches
- Distribuir provas do warmup em cada uma das salas
- Fixar mapas com o layout da sala na porta da sala de competićão (para identificaćão dos times e dos melancias
- Encher muitos balões: nos primeiros 40 minutos de competićão a demanda por balões é muito alta. Os times logo identificam os problemas mais fáceis e a grande maioria dos times passam um ou dois problemas. Por isso é geralmente impossível encher balão sob demanada e acompanhar o ritmo de entrega. Para não haver confusão e demora na entrega dos balões no início da competićão, é necessário haver um grande número de baões previamente enchidos para cada cor (um buffer bem gordo). Quanto número de balões enchidos nesse ponto é proporcional a tranquilidade da prova.
- Distribuir papel com o login do time e com a senha de acesso ao boca

Antes da prova

- Distribuir a prova verdadeira por todas as mesas


# Outras consideraćões

- O warmup e a primeira hora e meia da competićão é a que mais demanda staff:
	- Um grande número de balões é entregue na primeira hora de competićão, pois há  uns 4 problemas fáceis que são resolvidos pela grande maioria dos times
	- Problemas com login, problemas de rede e queda do servidor acontecem nesse momento por que é o momento de maior carga para o servidor e porque é o momento inicial dos competidores com o sistema. Muitos competidores estão usando o boca pela primeira vez no warmup. 
- Produzir balões com a logo da maratona paulista e a letra do problema
	- A maratona paulista tem um número alto de problema, mais de 10. Fica difícil encontrar 10 cores bem distintas. Além disso, o tom da cor muda se a bexiga foi muito inflada ou pouco inflada.

## Documentos para produzir

- Plaquinha: plaquinha com identificaćão do time que será fixado ao computador do time
- tabela/planilha dos organizadores: mapeia login do boca -> (nome do time , sala de competićão). 
	- Essa tabela deve ser ordenada pelo login do time
	- Cada melancia terá uma cópia dessa tabela
	- Uma cópia dessa tabela será fixada na sala dos balões e dos juízes
- tabela/planilha de divulgaćão: mapeia nome do time -> sala de competićão
	- tabela ordenada pelo nome do time
	- Essa tabela será fixada em um local público perto do credendimamento para os competidores encontrarem sua sala de competićão
	- Essa tabela tbm será fixada na sala dos coaches
- layout da sala: 
	- Para cada sala de competićão, desenhe a distribuićão dos times pela sala
	- esse layout será fixado na entrada da sala de competicão (serve para a localizaćão dos competidores e melancias)


