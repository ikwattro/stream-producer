# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
[markdownlint](https://dlaa.me/markdownlint/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.3.1] - 2021-01-20

### Added in 1.3.1

- Added support for websocket: `websocket-to-kafka`, `websocket-to-rabbitmq`, `websocket-to-sqs`,`websocket-to-sqs-batch`, `websocket-to-stdout`

## [1.3.0] - 2021-01-19

### Added in 1.3.0

- Microbatching for RabbitMQ, Kafka, and SQS. The batch of records is formatted as a json array
  - SENZING_RECORDS_PER_MESSAGE is the number of records to include in a single message.

## [1.2.3] - 2020-10-09

### Added in 1.2.3

- Support for Governor
- Support for environment variables:
  - `SENZING_RABBITMQ_ROUTING_KEY`
  - `SENZING_RABBITMQ_USE_EXISTING_ENTITIES`
  - `SENZING_RECORD_IDENTIFIER`
  - `SENZING_RECORD_SIZE_MAX`

## [1.2.2] - 2020-07-30

### Added in 1.2.2

- Added support for gzip: `gzipped-json-to-kafka`, `gzipped-json-to-rabbitmq`, `gzipped-json-to-sqs`, `gzipped-json-to-sqs-batch`, `gzipped-json-to-stdout`

## [1.2.1] - 2020-07-28

### Added in 1.2.1

- Monitoring metrics:  input_counter_rate_interval, input_counter_rate_total, output_counter_rate_interval, output_counter_rate_total
- Exit metric: rate

## [1.2.0] - 2020-07-24

### Added in 1.2.0

- Subcommands:  avro-to-sqs-batch, csv-to-sqs-batch, json-to-sqs-batch, and parquet-to-sqs-batch

## [1.1.1] - 2020-06-23

### Fixed in 1.1.1

- Bad variable

## [1.1.0] - 2020-06-19

### Added to 1.1.0

- Support for AWS SQS queue.

## [1.0.0] - 2020-06-18

### Added to 1.0.0

- Initial functionality
  - File formats: JSON, CSV, Avro, Parquet
  - Queues: RabbitMQ, Kafka, STDOUT
