# This is a list of tools/library that dotnet developer need to know. (2025)

## Version Control
1. Git                      ★★★★★
2. GitHub                   ★★★★★

## Online Resource
1. StackOverflow            ★★★★★
2. Copilot                  ★★★

## IDE
1. Visual Studio Code       ★★★★★
2. Visual Studio            ★★★
3. Rider                    ★★★★

## Language
1. C# 13                    ★★★★★
2. .Net 9                   ★★★★★
3. .Net Cli                 ★★★
4. .Net Aspire (integrated with Docker) ★★★★

## Solid Principles
1. Single Responsibility
2. Open-Closed
3. Liskov Substitution (The use of interface, allow substituting different class for testing)
4. Interface Segregation (Split methods by interfaces)
5. Dependency Inversion (For architecture, project should reference abstraction instead of implementation (ie. interface/abstract class)).
6. DRY (Don't repeat yourself, depends on context, sometime it is better to copy paste without causing over engineering or it is not worth the effort)
7. YAGNI (You aren't gonna need it, add feature only when you need it)
8. KISS (Keep it Simple and straightforward, imply coding standard and clean code)

## .Net
1. Web API
2. Routing
3. Middleware
4. Filters
5. Configuration
6. Authentication (authenticate the user through login, ie give token/cookies)
7. Authorization (authorize user to access resource, ie give credential/claims)
8. Dependency Injection

## Database
1. PostgreSql               ★★★★★
2. SQL Server               ★★★★

## API
1. Rest API
2. Hot Chocolate (GraphQL)
3. gRPC (http2)

## ORM
1. Entity Framework Core
2. Dapper

## NoSQL
1. Redis                    ★★★★★
2. AWS DynamoDB             ★★★★
3. Azure CosmosDB           ★★★★
4. Elastic Search           ★★★★

## Caching
1. Output Caching
2. Response Caching
3. Redis

## Logging
1. Microsoft.Extension.Logging
2. Serilog

## Message Queue
1. Azure service bus        ★★★★★
2. AWS SQS/SNS              ★★★★
3. RabbitMQ                 ★★★★

## Unit Testing (Testing individual method with mocking value).
1. MsTest/xUnit
2. Mocking (Moq/NSubstitute)
3. Assertion (FluentAssertions/Shouldly)
4. TestDataGeneration (Bogus/AutoFixture)

## Integration Testing (Testing the whole feature/Endpoint)
1. WebApplicationFactory (TestContainer)

## API Documentation
1. OpenAPI

## Background Task
1. Background Service (native)

## Monitoring & Telemetry
1. OpenTelemetry
2. Grafana 
3. ELK Stack
4. Prometheus

## Container
1. Docker
2. Kubernetes

## Clouds
1. Azure/AWS
2. Serverless (Azure Function/AWS Lambda)
3. File Storage (Azure Storage/AWS S3)

## CICD
1. GitHub Actions
2. Azure Pipeline

## Libraries
1. Polly (Retry process)
2. FluentValidation (Request body validation)
3. MediatR (can be implemented by yourself)

## DevOps
1. Terraform
