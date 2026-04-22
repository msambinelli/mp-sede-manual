
# Maratona de Programação - Manual de Sede

Este manual consolida as principais orientações para organizar uma sede da Maratona (Paulista?) de Programação. O objetivo é apoiar a preparação da infraestrutura, a definição da equipe, a organização dos espaços e a execução dos fluxos operacionais no dia da competição.

O documento está organizado como um guia prático. Cada sede deve adaptar as recomendações ao número de times, ao layout do local, ao parque de máquinas disponível e às regras específicas da edição.

## 1. Softwares

### 1.1 BOCA

O **BOCA** (Boca Online Contest Administrator) é a aplicação web usada para administrar a competição. Por meio dele, os times submetem soluções, acompanham o resultado das avaliações e solicitam serviços como impressão e entrega de balões. A equipe de organização também usa o sistema para acompanhar submissões, controlar o placar e operar a prova.

- Repositório oficial: https://github.com/cassiopc/boca
- Tutorial de instalação: https://www.youtube.com/watch?v=Hp-bL2Ws8M8

Recomendações operacionais:

- Tenha pelo menos duas pessoas com bom conhecimento do BOCA, sendo ao menos uma da sede local.
- Documente previamente os dados de acesso, os endereços dos servidores e os usuários administrativos.
- Evite depender de uma única pessoa para operar ou corrigir problemas no sistema.
- Realize um teste de carga antes da competição, preferencialmente com participação dos times inscritos.

Uma estratégia para verificar se a infraestrutura do BOCA suportará a carga do dia da competição é a realização de um _warm-up_ online no fim de semana anterior ao evento. Esse esquenta pode utilizar problemas de fontes públicas, como SPOJ ou Codeforces. O objetivo central é submeter o sistema a uma carga próxima da real, permitindo identificar previamente eventuais falhas, como limitações de capacidade ou instabilidades. Caso esses problemas ocorram, haverá tempo hábil para corrigi-los antes da competição oficial.

Além de seu papel técnico, o _warm-up_ também beneficia os competidores, ao possibilitar a familiarização com o ambiente do BOCA. Recomenda-se, contudo, que o formato do esquenta seja intencionalmente distinto da prova oficial: duração mais curta (cerca de duas horas), menor número de problemas e nível médio de dificuldade mais acessível. Essa diferenciação reduz comparações diretas entre o desempenho no _warm-up_ e as expectativas para a competição principal. Dessa forma, preserva-se o valor do teste tanto para a organização quanto para os participantes, ao mesmo tempo em que se minimiza o risco de desmotivação decorrente de um desempenho insatisfatório no esquenta.

#### Pendencias

- Seria interessante ver se existe alguma maneira de testar a carga do BOCA via scripts

### 1.2 Maratona Linux

O **Maratona Linux** é uma distribuição Linux personalizada para competições de programação. Ela deve ser usada nas máquinas dos competidores para garantir um ambiente uniforme, controlado e com as ferramentas necessárias para a prova, como compiladores, editores e bibliotecas padrão.

- Repositório oficial: https://github.com/maratona-linux/maratona-linux

Recomendações de preparação:

- Faça a instalação com alguns dias de antecedência, pois o processo pode ser lento e pode sobrecarregar o servidor de download.
- Após a cópia local da instalação, o software não precisa ser baixado novamente naquela máquina.
- Teste o Maratona Linux em todos os tipos de máquina que serão usados na competição.
- Tenha atenção especial com laboratórios heterogêneos, placas de vídeo offboard e, em particular, placas NVIDIA.
- Prepare vários pendrives de boot para acelerar a inicialização das máquinas no dia da competição.
- Confirme previamente a configuração de boot exigida pelo Maratona Linux, incluindo Secure Boot, UEFI e modo legacy.
- Pré-instale o ambiente em mais máquinas do que o número de times.

No dia da competição, todas as máquinas devem ser inicializadas com o pendrive do Maratona Linux. O sistema irá localizar a instalação previamente copiada, verificar sua integridade e continuar a execução a partir da versão instalada na máquina.

Sempre que possível, deixe uma máquina reserva próxima a cada time ou, ao menos, um conjunto de máquinas reservas prontas para uso. Problemas em computadores de competidores são comuns; a realocação rápida reduz o impacto sobre a prova.

Pendência a confirmar:

- Definir quem será responsável por gerar ou disponibilizar a versão customizada do Maratona Linux para a edição.

### 1.3 Maratona Animeitor Rust

O **Maratona Animeitor Rust** é usado na cerimônia de premiação para apresentar a classificação final de forma visual e dinâmica. Ele contribui para tornar a divulgação dos resultados mais envolvente para o público.

- Repositório oficial: https://github.com/wuerges/maratona-animeitor-rust

Recomendações operacionais:

- Teste o Animeitor antes do evento com uma base de dados de exemplo.
- Confirme se o laptop da apresentação consegue se conectar ao projetor ou telão.

## 2. Espaços Necessários

A sede deve reservar e preparar todos os espaços necessários para receber competidores, coaches, juízes, equipe técnica e equipe de apoio.

### 2.1 Anfiteatro ou auditório

Usado para recepção dos competidores, abertura e premiação.

Deve conter:

- Telão ou projetor.
- Microfone.
- Entrada HDMI ou adaptadores adequados para ligar um laptop.
- Espaço suficiente para competidores, coaches, organizadores e convidados.

### 2.2 Sala dos juízes

Espaço reservado para juízes, administradores do BOCA e pessoas responsáveis pela operação técnica da prova.

Deve conter:

- Ambiente calmo e com acesso controlado.
- Computadores com os mesmos compiladores disponíveis aos competidores, ou instalações do Maratona Linux.
- Acesso ao BOCA por rede cabeada ou Wi-Fi.
- Condições para que juízes usem seus próprios notebooks, quando necessário.

Antes da competição, confirme se a rede da sala dos juízes consegue acessar o BOCA. Em muitas universidades, redes cabeadas e redes Wi-Fi podem ser isoladas entre si.

### 2.3 Sala dos coaches

Espaço onde os coaches acompanham a competição.

Recomendações:

- Disponibilizar Wi-Fi.
- Projetar o placar ou exibi-lo em uma TV.
- Oferecer água, café e petiscos.
- Fixar informações úteis, como mapa das salas e cronograma do evento.

### 2.4 Sala de balões e impressão

Espaço operacional onde são preparados os balões e processados os pedidos de impressão.

Deve conter:

- Computador para o operador de impressão.
- Computador para o operador de balões.
- Impressora.
- Grampeador, papel, cartões pautados.
- Escaninhos separados para impressões e balões.
- Mapa dos times, com login do BOCA, nome do time e sala.
- Espaço para armazenar balões já inflados por cor ou identificação.
- Tomada para ligar a máquina de inflar balões.

### 2.5 Salas de competição

Salas onde os times realizam a prova.

Cada sala deve conter:

- Máquinas preparadas com Maratona Linux.
- Máquinas reservas.
- Identificação visível de cada time.
- Fiscal de prova.
- Layout fixado na porta, indicando a posição dos times.

### 2.6 Recepção e credenciamento

Local usado para receber participantes, confirmar presença e orientar os times.

Deve conter:

- Lista indicando a sala de cada time.
- Informações sobre abertura, warm-up, início da prova e premiação.
## 3. Equipamentos

A lista abaixo resume os principais equipamentos necessários.

- Um computador por time.
- Computadores reservas para realocação rápida.
- Ao menos dois computadores ou servidores para rodar o BOCA, conforme a arquitetura adotada.
- Um computador para o responsável técnico pelo BOCA.
- Um computador dedicado ao operador de impressão.
- Um computador dedicado ao operador de balões.
- Um computador para cada juiz que contenha todos os compiladores da competição.
- Um laptop para abertura, apresentações e execução do Animeitor na premiação.
- Impressora testada e com suprimentos suficientes.
- Pendrives de boot do Maratona Linux.
- Projetor ou telão, microfones, cabos e adaptadores.
- Máquina de encher balões, balões, fitas, cartões e materiais de apoio.

## 4. Equipe e Papéis

Organizar uma sede exige uma equipe numerosa. A demanda de pessoas é maior durante o warm-up e na primeira hora da competição, quando aparecem problemas de login, rede, acesso ao BOCA, impressões e grande volume de balões.

### 4.1 Coordenador da sede

Pessoa responsável pela organização geral da sede e pela tomada de decisão quando surgirem imprevistos.

Responsabilidades:

- Coordenar a preparação antes do evento.
- Distribuir funções entre as equipes.
- Resolver problemas operacionais no dia da competição.
- Ser o ponto central de comunicação entre organização local, juízes, equipe técnica e apoio.

### 4.2 Responsável de rede

Profissional que conhece a infraestrutura de rede do local.

Responsabilidades:

- Resolver problemas de conectividade e instabilidade de rede durante a prova.
### 4.3 Administradores do BOCA

Pessoas responsáveis pela configuração, monitoramento e operação do BOCA.

Recomendações:

- Ter pelo menos duas pessoas capacitadas.
- Manter uma pessoa da sede local entre os responsáveis.

### 4.4 Juízes

Equipe responsável por acompanhar a prova do ponto de vista técnico e julgar situações que exigem intervenção humana.

Responsabilidades:

- Acompanhar submissões e esclarecimentos.
- Responder dúvidas oficiais quando aplicável.
- Apoiar a validação do ambiente de competição.

### 4.5 Fiscais de prova

Pessoas que permanecem nas salas durante a competição.

Recomendações:

- Ter no mínimo um fiscal por sala.
- Considerar dois fiscais por sala durante o warm-up e a primeira hora da prova.
- Ajustar a quantidade de fiscais conforme o tamanho da sala e o número de times.

Responsabilidades:

- Acompanhar a execução da prova na sala.
- Acionar fiscais de corredor ou organizadores quando necessário.
- Orientar deslocamentos autorizados, como idas ao banheiro.
- Reportar problemas de máquina, rede ou comportamento.

### 4.6 Fiscais de corredor

Equipe de apoio que circula entre salas e atende chamados dos fiscais de prova.

Responsabilidades:

- Acompanhar competidores em deslocamentos autorizados.
- Chamar organizadores, equipe técnica ou responsáveis pelo BOCA.
- Apoiar a comunicação entre salas e organização central.

A quantidade necessária depende do layout do local e da distância entre salas.

### 4.7 Equipe de logística, ou "melancias"

Os "melancias" são as pessoas responsáveis pelo transporte interno de balões, impressões e outros materiais.

Responsabilidades:

- Retirar impressões no escaninho de impressão e entregá-las aos times corretos.
- Retirar cartões de balões, pegar o balão correspondente e entregá-lo ao time correto.

A quantidade necessária varia conforme o número de times, a quantidade de salas e a distância entre os espaços.

### 4.8 Operador de impressão

Pessoa responsável por processar os pedidos de impressão recebidos pelo BOCA.

Responsabilidades:

- Receber solicitações de impressão.
- Baixar os arquivos.
- Imprimir e grampear a impressão.
- Consultar na planilha o nome do time e sala associado ao login do time e anotar à caneta essas informações na impressão.
- Colocar a impressão no escaninho de impressão para ser retirada pelos melancias.

### 4.9 Operador de balões

Pessoa responsável por processar os pedidos de balões.

Responsabilidades:

- Receber solicitações de balões.
- Consultar na planilha o nome do time e sala associado ao login do time.
- Registrar o nome do time, sala e cor do balão no cartão pautado.
- Colocar o pedido no escaninho dos balões para retirada pelos melancias.

### 4.10 Baloeiros

Pessoas responsáveis por inflar e organizar os balões.

Recomendações:

- Ter no mínimo duas pessoas nessa função.
- Manter um estoque inicial de balões prontos antes da prova.

## 5. Fluxos Operacionais

### 5.1 Fluxo de impressão

1. O operador de impressão recebe a solicitação no BOCA.
2. O operador baixa o arquivo enviado pelo time.
3. O operador imprime o arquivo.
4. O operador grampeia as folhas.
5. O operador consulta o mapa que relaciona login do BOCA, nome do time e sala.
6. O operador anota manualmente o nome do time e sala na impressão.
7. O operador coloca a impressão no escaninho de impressão.
8. O operador marca no BOCA que o arquivo foi impresso.
9. Um melancia retira a impressão e entrega ao time correto.

### 5.2 Fluxo de balões

1. O operador de balões recebe a solicitação no BOCA.
2. O operador consulta a tabela que relaciona login do BOCA, nome do time e sala.
3. O operador registra em um cartão pautado o nome do time, sala e cor do balão.
4. O operador coloca o cartão no escaninho de balões.
5. O operador marca no BOCA que o balão foi entregue.
6. Um melancia retira o cartão, pega o balão correspondente e entre ao time correto.

Os baloeiros devem trabalhar em paralelo, mantendo sempre um estoque mínimo de balões já inflados para cada cor ou identificação.

## 6. TODO Cronograma Operacional

### 6.1 Antes do dia da competição

- Definir todos os espaços que serão usados.
- Confirmar acesso às salas, auditório e laboratórios.
- Preparar e testar o BOCA.
- Preparar e testar o Maratona Linux nas máquinas.
- Testar rede cabeada e Wi-Fi nos espaços relevantes.
- Testar impressora, projetor, microfones e equipamentos de apoio.
- Preparar pendrives de boot.
- Produzir placas de identificação dos times.
- Produzir mapas, tabelas e layouts de sala.
- Definir a escala da equipe.
- Fazer um warm-up online para testar carga e operação.

### 6.2 No dia da competição, antes do warm-up

O trabalho no dia da competição deve começar cedo, idealmente entre três e quatro horas antes do início previsto da prova.

Checklist recomendado:

- Inicializar o Maratona Linux em todas as máquinas de competição, inclusive reservas.
- Organizar o auditório ou anfiteatro.
- Distribuir placas de identificação dos times nas máquinas.
- Fixar materiais de divulgação e sinalização.
- Abrir e organizar todas as salas.
- Distribuir materiais operacionais, como balões, impressora, café,  papel, fita, caneta e etc.
- Ligar computadores, impressoras, máquina de encher balões, projetores e microfones.
- Preparar água, café e lanches da sala dos coaches.
- Distribuir as provas do warm-up nas salas.
- Fixar o layout de cada sala na respectiva porta.
- Distribuir os logins e senhas do BOCA aos times.
- Inflar uma quantidade inicial significativa de balões.

A preparação antecipada dos balões é especialmente importante. Nos primeiros 40 minutos da competição, a demanda costuma ser muito alta, pois os times identificam rapidamente os problemas mais acessíveis. Se os balões forem inflados apenas sob demanda, a entrega pode atrasar e gerar confusão. Um estoque inicial robusto reduz esse risco.

### 6.3 Durante o warm-up

- Confirmar que todos os times conseguem acessar o BOCA.
- Verificar se a impressão está funcionando.

### 6.4 Após o warm-up e antes da prova oficial

- Distribuir a prova oficial em todas as mesas.

### 6.5 Após a prova

- Registrar problemas ocorridos e sugestões para a próxima edição.
- Salvar logs, placares e informações relevantes da competição.

## 7. Documentos e Materiais a Produzir

### 7.1 Placas de identificação dos times

Placas fixadas nas máquinas ou mesas dos competidores.

Devem conter:

- Nome do time e universidade

### 7.2 Tabela dos organizadores

Planilha interna que relaciona login do BOCA, nome do time e sala de competição.

Recomendações:

- Ordenar pelo login do BOCA.
- Entregar cópias à equipe de logística.
- Fixar uma cópia na sala de balões e impressão.
- Fixar uma cópia na sala dos juízes, se necessário.
- Pode ser mais prático disponibilizar o arquivo do Excel para os operadores de impressão e balão buscarem o time usando Ctrl+f

### 7.3 Tabela de divulgação

Planilha pública que relaciona nome do time e sala de competição.

Recomendações:

- Ordenar pelo nome do time.
- Fixar em local visível próximo ao credenciamento.
- Fixar uma cópia na sala dos coaches.
- Evitar divulgar senhas ou informações internas nessa versão.

### 7.4 Layout das salas

Mapa indicando a distribuição dos times em cada sala de competição.

Recomendações:

- Criar um layout para cada sala.
- Fixar o layout na entrada da sala.
- Usar o mesmo layout para orientar fiscais e equipe de logística.

### 7.5 Credenciais de acesso

Documento ou envelope entregue a cada time com as informações de acesso ao BOCA.

Deve conter:

- Login do time.
- Senha.
- URL do BOCA.
- Instruções básicas de acesso, se necessário.

### 7.6 Tabela de Alocação de Staff

Documento que define, de forma clara e organizada, as responsabilidades, os locais de atuação e os horários de trabalho de cada membro da equipe de organização ao longo da competição.

## 8. Boas Práticas e Pontos de Atenção

### 8.1 Dimensionamento da equipe

O _warm-up_ e a primeira hora da competição concentram um grande número de eventos simultâneos, como dúvidas de acesso, problemas de rede, elevado volume de submissões (e consequente fluxo de balões), pedidos de impressão e eventuais falhas nas máquinas. Dessa forma, a alocação da equipe deve ser cuidadosamente dimensionada para esse período crítico, garantindo capacidade de resposta rápida e evitando sobrecarga operacional.

### 8.2 Balões personalizados

A maratona pode ter mais de dez problemas, o que dificulta usar apenas cores distintas de balões. Além disso, a tonalidade pode variar conforme o nível de inflação da bexiga.

Uma alternativa é produzir balões com a logo da competição e a letra do problema. Isso reduz ambiguidades e confusão na entrega de balões.

### 8.3 Plano de contingência

Antes do evento, pense sobre procedimentos para os principais riscos:

- Queda do BOCA.
- Instabilidade de rede.
- Falha de impressora.
- Falha em máquina de competidor.
- Falta de Internet (caso o BOCA seja hospedado fora da rede local)
- Problemas com projetor ou telão.
- Ausência inesperada de uma pessoa-chave da equipe.

### 8.4 Comunicação interna

Defina previamente um canal de comunicação entre coordenação, juízes, fiscais, equipe técnica e apoio. O canal pode ser um grupo de mensagens ou outro meio adequado ao local.

### 8.5 Registro de incidentes

Mantenha um registro simples de incidentes ocorridos durante o dia. Para cada incidente, anote horário, local, descrição, pessoa responsável e solução adotada. Esse histórico ajuda em decisões durante a prova e melhora a organização das próximas edições.

## 9. Pendências

- Confirmar quem cria ou disponibiliza a versão customizada do Maratona Linux para a edição.
- Definir a arquitetura final do BOCA, incluindo quantidade de servidores, backups e responsáveis.
- Definir a quantidade mínima de pessoas por função conforme número de times e layout da sede.
- Definir templates/exemplos dos documentos impressos: placas, tabelas, layouts e credenciais.
- Confecção de troféus
- Tutorial sobre problemas?
