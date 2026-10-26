# Correção da AV1 — GPTI — FluxoPark

Repositório: https://github.com/juanmends/fluxopark-gpti (commit `17f7f527`, 05/10/2026 14h00).

Artefatos: `business-case-fluxopark.md`, `termo-de-abertura-fluxopark.md`, `plano-de-projeto-fluxopark.md` e `dicionario-eap-fluxopark.md`, com os Gantt e a alocação individual em `cronograma-*.png` e `cronograma-*.html`.

A nota é do Grupo B de GPTI e vale para cada aluno do grupo. Nesta etapa, a ausência de commit não zera ninguém. O nome na atividade do cronograma é o contrato da etapa seguinte. A especificação de referência é o refinamento de PSW de 09/09/2026, corrigido na AV1 de PSW: CRUD de estacionamento e de vaga, pesquisar destino, reserva e pagamento, gestão de reservas, avaliar e emitir avaliações, sobre JSON Server.

| Aluno | Nota |
| --- | ---: |
| Maria Luisa Santiago Vieira | 89 |
| Ana Clara dos Santos Morais | 89 |
| Juan Silva Mendes | 89 |
| Manuela Ribeiro Rodrigues da Silva | 89 |
| Beatriz Daniel Manhães | 89 |

## Parte comum — 89/100

| Parte | Nota |
| --- | ---: |
| Business case | 10/10 |
| Termo de abertura | 14/15 |
| Escopo e EAP | 15/15 |
| Cronograma com nomes | 18/25 |
| Custo, partes e riscos | 15/15 |
| Dicionário da EAP | 13/15 |
| Um projeto só | 4/5 |

### Business case — 10/10

O caso traz problema, oportunidade, soluções existentes no mercado, objetivos com meta, alternativas com recomendação e análise econômica de 24 meses com VPL, TIR, ROI, payback, índice benefício-custo e sensibilidade. O investimento é o orçamento do plano, 540 h e R$ 10.400,40. A seção 12 separa o retorno de uma operação futura do retorno deste projeto, que é um MVP com pagamento em *sandbox*.

### Termo de abertura — 14/15

O termo nomeia o patrocinador e a gerente do projeto, Ana Clara, com autoridade e prestação de contas. Traz objetivos com quem mede, escopo dentro e fora, abordagem em duas etapas separadas pela AV1, marcos M1 e M2 com critério de aceite, critérios de encerramento e cancelamento, premissas, restrições, partes interessadas, riscos iniciais, orçamento e aprovação.

Desconto:

- 1 ponto. Os objetivos do MVP e o marco M2 incluem um teste piloto com 2 a 3 estacionamentos parceiros reais e metas de negócio medidas nele (tempo de estacionamento 30% menor, ocupação 20 pontos acima, adesão de 2 parceiros). A especificação de PSW é o protótipo; o piloto com parceiros reais fica fora dela.

### Escopo e EAP — 15/15

A declaração do escopo, os requisitos REQ-01 a REQ-11, a matriz CRUD, a matriz perfil × funcionalidade e a rastreabilidade cobrem as seis entregas da especificação. A EAP separa 1.4, frontend do marco 1 sobre `json-server`, de 1.5 e 1.6, backend Express com MongoDB e integração, com a regra de que nenhuma atividade de backend começa antes do aceite do M1. A remoção de estacionamento cabe ao administrador, como na matriz da PSW. Os pacotes do piloto (1.1.4 e 1.7.4) estão cobrados no termo.

### Cronograma com nomes — 18/25

A rede D01 a D18 e G01 a G12 tem predecessora FS ou SS, janela, duração, esforço e custo. Há caminho crítico, folga calculada para D05, conferência de três pontos em D07 e D15 e Gantt com dependências. A seção 5.5 tem, para cada aluno de PSW e cada semana, a tarefa e as horas, e os quatro passam pelo frontend e pelo backend.

Descontos:

- 5 pontos. A gestão não tem pessoa em nenhuma atividade. O plano diz que "os papéis individuais da equipe de gestão ainda não foram definidos"; G01 a G12 são da equipe, a seção 5.6 mostra a carga somada dos cinco e o Gantt de gestão é um bloco único. Beatriz, Juan, Manuela e Maria Luisa não têm uma tarefa de uma semana no nome.
- 1 ponto. Nas linhas D01 a D18, a atividade é "executada pelos quatro alunos em revezamento". A divisão por pessoa fica só na semana.
- 1 ponto. O plano não fixa datas de calendário. O M1 está na "semana 8" e o M2 na "semana 12", e o cronograma começa pelo protótipo das semanas 1 e 2, que o refinamento de 09/09 já entregou. A AV1 de 05/10 e o M2 de 30/11 não aparecem como datas.

### Custo, partes e riscos — 15/15

O orçamento parte da capacidade dos calendários (540 h a R$ 18,00), separa a linha de base de R$ 9.720,00, com 64 h de contingência distribuídas por evento de risco nomeado, da reserva gerencial de 7%, sob controle do patrocinador. A seção 6.2.1 confere o calendário com uma segunda estimativa pelo entregável e explica a diferença. O registro tem treze ameaças com probabilidade, impacto em horas, gatilho, contingência e responsável nominal, e a oportunidade OP01 com resposta. O engajamento tem matriz corrente e desejada, poder e interesse, plano e cadência de comunicação.

### Dicionário da EAP — 13/15

Cada pacote tem A, R e aceite observável, e cada pacote técnico tem um único aluno de PSW como A. O aceite é o da especificação: "Um estacionamento ou vaga cadastrado aparece na busca logo após o cadastro"; "no mock, a reserva só passa a confirmada depois do retorno da simulação de pagamento"; "Só uma reserva concluída pode ser avaliada".

Descontos:

- 1 ponto. Nos pacotes de gestão, o A é Ana Clara e o R é "Equipe de gestão" em todas as linhas. Beatriz, Juan, Manuela e Maria Luisa não aparecem no dicionário.
- 1 ponto. Nos pacotes técnicos, o R é "Equipe PSW" em todas as linhas, e o cronograma já tem a pessoa.

### Um projeto só — 4/5

Os quatro documentos usam o mesmo recorte, a mesma equipe, os mesmos marcos e os mesmos números: 540 h, R$ 9.720,00 de linha de base e R$ 10.400,40 de orçamento. Os códigos da EAP batem com o dicionário e com a coluna "Pacote" das atividades.

Desconto:

- 1 ponto. O pedido da AV1 era entregar no repositório de PSW. Os artefatos estão em `juanmends/fluxopark-gpti`, fora do repositório do grupo.

## O que esta nota deixa para a etapa seguinte

Em PSW, cada semana tem uma tarefa e as horas no nome de Daniel, Fernando, Ricardo e Walter, e cada pacote técnico tem um A nominal. Na gestão, o que se consegue cobrar é Ana Clara como A de todos os pacotes e dos riscos de gestão. Os outros quatro alunos de gestão não têm atividade, semana ou pacote no nome. A divisão dos papéis, que o plano deixa para depois, é a primeira coisa que o status da etapa seguinte precisa registrar.
