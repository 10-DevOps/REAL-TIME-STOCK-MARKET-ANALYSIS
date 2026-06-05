## Project Name: Real Time Stock Market Analysis

The project implements a real-time data pipeline that extracts stock data fom                                    vantage API, streams it through Apache Kafka, processes it with Apache Spark, and                                loads it into a postgres database.                                                                                        

All components are containerized with Docker for easy deployment.

### Data Pipeline Architecture
![Data Pipeline Architecture](./img/pipeline%20diagram.svg)


Project Tech Stack and Flow
   - `Kafka UI  inspect topics/messages.`
   - `API  poduces JSON events into Kafka.`
   - `Spark  consumes from Kafka, writes to Postgres.`
   - `Postgres  stores results for analystics.`
   - `pgAdmin  manage Postgres visually.`
   - `Power BI  external (connects to Postgres database).`