# Zuber

In this project I analyzed Zuber, a new ride-sharing company being launched in Chicago. My task is to find patterns in the information available. To understand passenger preferences and the impact of external factors on rides.
Working with a database, I analyzed data from competitors and tested a hypothesis about the impact of weather on trip frequency.


*The SQL part was made in the tripleten plataform, but the tasks and codes are in the SQL code parte in the files*

**Data description (SQL)**

A database with information on cab rides in Chicago:
* neighborhoods table: data on the city's neighborhoods
* name: name of the neighborhood
* neighborhood_id: neighborhood code
* cabs table: data on cabs
* cab_id: vehicle code
* vehicle_id: the technical identification of the vehicle
* company_name: the company that owns the vehicle
* trips table: data on rides
* trip_id: trip code
* cab_id: code of the vehicle operating the run
* start_ts: date and time of the start of the run (time rounded to the hour)
* end_ts: date and time of the end of the race (time rounded to the hour)
* duration_seconds: race duration in seconds
* distance_miles: distance covered in miles
* pickup_location_id: pickup neighborhood code
* dropoff_location_id: delivery neighborhood code
* weather_records table: weather data
* record_id: weather record code
* ts: records date and time (time rounded to the hour)
* temperature: temperature when the record was made
* description: brief description of the weather conditions, e.g. "light rain" or "sparse clouds"

**Python**

You now have these two CSVs:
project_sql_result_01.csv. 

**It contains the following data**
* company_name: name of the cab company
* trips_amount: the number of runs for each cab company from November 15 to 16, 2017.

project_sql_result_04.csv. 
**It contains the following data**
* dropoff_location_name: Chicago neighborhoods where the runs ended
* average_trips: the average number of trips that ended in each neighborhood in November 2017.


Test the hypothesis: "The average length of rides from the Loop to O'Hare International Airport changes on rainy Saturdays."

**Conclusion**
Passenger preferences are:
1- Loop 2- River North 3- Streeterville 4- West Loop 5- O'Hare 6- Lake View 7- Grant Park 8- Museum Campus 9- Gold Coast 10- Sheffield & DePaul

External factors do have an impact, both on the length of journeys (proven in the statistical test) and on the number of runs (difference in rows of the dataframe filtered by good weather (888) and bad weather (180). With a total of 708 more runs on days with good weather).


# Zuber

Neste projeto, analisei a Zuber, uma nova empresa de compartilhamento de caronas que está sendo lançada em Chicago. Minha tarefa é encontrar padrões nas informações disponíveis. Entender as preferências dos passageiros e o impacto de fatores externos sobre as caronas.
Trabalhando com um banco de dados, analisei dados de concorrentes e testei uma hipótese sobre o impacto do clima na frequência das viagens.


*A parte do SQL foi feita na plataforma tripleten, mas as tarefas e os códigos estão na parte do código SQL nos arquivos

**Descrição dos dados (SQL)**

Um banco de dados com informações sobre viagens de táxi em Chicago:
* Tabela de bairros: dados sobre os bairros da cidade
* nome: nome do bairro
* neighborhood_id: código do bairro
* Tabela cabs: dados sobre os táxis
* cab_id: código do veículo
* vehicle_id: a identificação técnica do veículo
* company_name: a empresa proprietária do veículo
* Tabela trips: dados sobre viagens
* trip_id: código da viagem
* cab_id: código do veículo que está operando a corrida
* start_ts: data e hora do início da corrida (hora arredondada para a hora)
* end_ts: data e hora do final da corrida (hora arredondada para a hora)
* duration_seconds: duração da corrida em segundos
* distance_miles: distância percorrida em milhas
* pickup_location_id: código do bairro de coleta
* dropoff_location_id: código do bairro de entrega
* Tabela weather_records: dados meteorológicos
* record_id: código do registro meteorológico
* ts: data e hora dos registros (hora arredondada para a hora)
* temperatura: temperatura quando o registro foi feito
* description: breve descrição das condições meteorológicas, por exemplo, "chuva leve" ou "nuvens esparsas".

**Python**

Agora você tem esses dois CSVs:
project_sql_result_01.csv. 

**Ele contém os seguintes dados**
* company_name: nome da empresa de táxi
* trips_amount: o número de corridas para cada empresa de táxi de 15 a 16 de novembro de 2017.

project_sql_result_04.csv. 
**Contém os seguintes dados**
* dropoff_location_name: bairros de Chicago onde as corridas terminaram
* average_trips: o número médio de viagens que terminaram em cada bairro em novembro de 2017.


Teste a hipótese: "A duração média das viagens do Loop para o Aeroporto Internacional O'Hare muda em sábados chuvosos."

**Conclusão**
As preferências dos passageiros são:
1- Loop 2- River North 3- Streeterville 4- West Loop 5- O'Hare 6- Lake View 7- Grant Park 8- Museum Campus 9- Gold Coast 10- Sheffield & DePaul

Os fatores externos têm um impacto, tanto na duração das viagens (comprovado no teste estatístico) quanto no número de viagens (diferença nas linhas do quadro de dados filtradas por tempo bom (888) e tempo ruim (180). Com um total de 708 corridas a mais em dias com tempo bom).
