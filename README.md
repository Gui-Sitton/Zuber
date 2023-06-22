# Zuber

*Este foi um projeto com duas etapas, a primeira eu tive que obter e trasnformar dados usando sql na própria plataforma de ensino e a segunda usei python para testar as hipóteses

Sou aluno da TripleTen no curso de Ciência de Dados, estou divulgando projetos que desenvolvi para meu portifólio. Este é o sexto projeto.

Você está trabalhando como analista da Zuber, uma nova empresa de compartilhamento de caronas que está sendo lançada em Chicago. Sua tarefa é encontrar padrões nas informações disponíveis. Você quer entender as preferências dos passageiros e o impacto de fatores externos nas corridas.
Trabalhando com um banco de dados, você analisará dados de concorrentes e testará uma hipótese sobre o impacto do clima na frequência das viagens.

*Este foi um projeto com duas etapas, a primeira eu tive que obter e trasnformar dados usando sql na própria plataforma de ensino e a segunda usei python para testar as hipóteses

(SQL)
**Descrição dos dados**
Um banco de dados com informações sobre corridas de táxi em Chicago:
* tabela neighborhoods: dados sobre os bairros da cidade
* name: nome do bairro
* neighborhood_id: código do bairro
* tabela cabs: dados sobre os táxis
* cab_id: código do veículo
* vehicle_id: a identificação técnica do veículo
* company_name: a empresa proprietária do veículo
* tabela trips: dados sobre corridas
* trip_id: código da corrida
* cab_id: código do veículo que opera a corrida
* start_ts: data e hora do início da corrida (tempo arredondado para a hora)
* end_ts: data e hora do final da corrida (tempo arredondado para a hora)
* duration_seconds: duração da corrida em segundos
* distance_miles: distância percorrida em milhas
* pickup_location_id: código do bairro de retirada
* dropoff_location_id: código do bairro de entrega
* tabela weather_records: dados sobre o clima
* record_id: código de registro meteorológico
* ts: grava data e hora (tempo arredondado para a hora)
* temperature: temperatura quando o registro foi feito
* description: breve descrição das condições meteorológicas, ex. "chuva leve" ou "nuvens esparsas"

(python)
Agora você tem estes dois CSVs:
project_sql_result_01.csv. 

**Ele contém os seguintes dados:**
* company_name: nome da empresa de táxi
* trips_amount: o número de corridas para cada empresa de táxi de 15 a 16 de novembro de 2017.

project_sql_result_04.csv. 
**Ele contém os seguintes dados:**
* dropoff_location_name: bairros de Chicago onde as corridas terminaram
* average_trips: o número médio de viagens que terminaram em cada bairro em novembro de 2017.


Teste a hipótese: "A duração média dos passeios do Loop para o Aeroporto Internacional O'Hare muda nos sábados chuvosos."

**Conclusão**
As preferências dos passageiros são:
1- Loop 2- River North 3- Streeterville 4- West Loop 5- O'Hare 6- Lake View 7- Grant Park 8- Museum Campus 9- Gold Coast 10- Sheffield & DePaul

Fatores externam impactam sim, tanto no tempo de duração das viagens (comprovado no teste estatístico), quanto no número de corridas (diferença de linhas do dataframe filtrado pelo tempo bom (888) com o tempo ruim (180). Com um total de 708 corridas a mais em dias com o clima bom).
