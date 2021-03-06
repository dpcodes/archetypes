# `swagger_client`

> The `Quantity` archetype represents an amount of something measured according to some standard of measurement.

## Compliance with standards and proposals

<table>   <thead>     <tr><th>Standard</th><th>Contents</th></tr>   </thead>   <tfoot>   </tfoot>   <tbody>     <tr>       <td><a href=\"http://www.bipm.org/en/measurement-units/\">SI</a></td>       <td>International System of Units&mdash;Bureau International des Poids et Mesures (BIPM).</td>     </tr>   </tbody> </table>  


---  


## Business archetypes defined

> "A business archetype is a primordial thing that occurs consistently and universally in business domains and business software systems." (Arlow & Neustadt, [_Enterprise patterns and MDA: building better software with archetype patterns and UML_](https://www.amazon.com/Enterprise-Patterns-MDA-Building-Archetype/dp/032111230X), 2006, p. 5)  


## Explore other business archetype patterns

[Open a Swagger-UI](http://api.swindle.net/swagger-ui/#/) instance, then copy and paste the following Swagger specification URLs into the "Explore" text field and select the "Explore" button for additional APIs.

1. `Locale`: http://api.swindle.net/archetypes/v1/schemas/locale/locale.swagger.json
2. `Party`: http://api.swindle.net/archetypes/v1/schemas/party/party.swagger.json
3. `Quantity`: http://api.swindle.net/archetypes/v1/schemas/quantity/quantity.swagger.json


---

 ## About

This SDK is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build package: io.swagger.codegen.languages.RubyClientCodegen

## Installation

### Build a gem

To build the Ruby code into a gem:

```shell
gem build swagger_client.gemspec
```

Then either install the gem locally:

```shell
gem install ./swagger_client-1.0.0.gem
```
(for development, run `gem install --dev ./swagger_client-1.0.0.gem` to install the development dependencies)

or publish the gem to a gem hosting service, e.g. [RubyGems](https://rubygems.org/).

Finally add this to the Gemfile:

    gem 'swagger_client', '~> 1.0.0'

### Install from Git

If the Ruby gem is hosted at a git repository: https://github.com/YOUR_GIT_USERNAME/YOUR_GIT_REPO, then add the following in the Gemfile:

    gem 'swagger_client', :git => 'https://github.com/YOUR_GIT_USERNAME/YOUR_GIT_REPO.git'

### Include the Ruby code directly

Include the Ruby code directly using `-I` as follows:

```shell
ruby -Ilib script.rb
```

## Getting Started

Please follow the [installation](#installation) procedure and then run the following code:
```ruby
# Load the gem
require 'swagger_client'

api_instance = SwaggerClient::LaborApi.new

body = SwaggerClient::SystemOfUnits3.new # SystemOfUnits3 | The new `Unit` object to be added.<br><br>**Important**: The `name` of the labor `Unit`, i.e., \"`work-hour`\".<ul><li>**Case-sensitivity**: `name's` value is **case-sensitive**. For example, \"`work-hour`\" will return data, but \"Work-Hour\" will result in an HTTP status code of 404 (`NotFoundError`).<li>**Format**: `name's` value must be given in [**kebab case**](https://runkit.com/gregswindle/59a1c3805d3740001245a72d). For example, \"`work-hour`\" will return data, but \"work hour\" (with whitespace) or \"`WorkHour`\" (in [`PascalCase`](http://wiki.c2.com/?PascalCase)) will result in an HTTP status code of 404 (`NotFoundError`).


begin
  #Create an new Unit of Labor.
  result = api_instance.create_labor_unit(body)
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling LaborApi->create_labor_unit: #{e}"
end

```

## Documentation for API Endpoints

All URIs are relative to *http://api.swindle.net/archetypes/v1/quantities*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*SwaggerClient::LaborApi* | [**create_labor_unit**](docs/LaborApi.md#create_labor_unit) | **POST** /systems-of-units/labor | Create an new Unit of Labor.
*SwaggerClient::LaborApi* | [**get_labor_unit_by_name**](docs/LaborApi.md#get_labor_unit_by_name) | **GET** /systems-of-units/labor/{name} | Retrieve a metric or unit by name.
*SwaggerClient::SIInternationalSystemOfUnitsApi* | [**get_si_base_unit_by_name**](docs/SIInternationalSystemOfUnitsApi.md#get_si_base_unit_by_name) | **GET** /systems-of-units/SI/base-units/{name} | Retrieve a metric or unit by its SI name.
*SwaggerClient::SystemsOfUnitsApi* | [**create_system_of_units**](docs/SystemsOfUnitsApi.md#create_system_of_units) | **POST** /systems-of-units | Create an new SystemOfUnits.
*SwaggerClient::SystemsOfUnitsApi* | [**get_system_of_units_by_name**](docs/SystemsOfUnitsApi.md#get_system_of_units_by_name) | **GET** /systems-of-units/{name-of-system} | Retrieve a specific system of units by name.
*SwaggerClient::SystemsOfUnitsApi* | [**get_systems_of_units**](docs/SystemsOfUnitsApi.md#get_systems_of_units) | **GET** /systems-of-units | Retrieve all systems of units.


## Documentation for Models

 - [SwaggerClient::Ampere](docs/Ampere.md)
 - [SwaggerClient::BadRequestError](docs/BadRequestError.md)
 - [SwaggerClient::Candela](docs/Candela.md)
 - [SwaggerClient::DerivedUnit](docs/DerivedUnit.md)
 - [SwaggerClient::DerivedUnitTerm](docs/DerivedUnitTerm.md)
 - [SwaggerClient::DerivedUnitTerm1](docs/DerivedUnitTerm1.md)
 - [SwaggerClient::ForbiddenError](docs/ForbiddenError.md)
 - [SwaggerClient::InlineResponse400](docs/InlineResponse400.md)
 - [SwaggerClient::InlineResponse401](docs/InlineResponse401.md)
 - [SwaggerClient::InlineResponse403](docs/InlineResponse403.md)
 - [SwaggerClient::InlineResponse404](docs/InlineResponse404.md)
 - [SwaggerClient::InlineResponse405](docs/InlineResponse405.md)
 - [SwaggerClient::Kelvin](docs/Kelvin.md)
 - [SwaggerClient::Kilogram](docs/Kilogram.md)
 - [SwaggerClient::Meter](docs/Meter.md)
 - [SwaggerClient::MethodNotAllowedError](docs/MethodNotAllowedError.md)
 - [SwaggerClient::Metric](docs/Metric.md)
 - [SwaggerClient::Metric1](docs/Metric1.md)
 - [SwaggerClient::Mole](docs/Mole.md)
 - [SwaggerClient::NotFoundError](docs/NotFoundError.md)
 - [SwaggerClient::Quantity](docs/Quantity.md)
 - [SwaggerClient::QuantityRoundingPolicy](docs/QuantityRoundingPolicy.md)
 - [SwaggerClient::RoundingPolicy](docs/RoundingPolicy.md)
 - [SwaggerClient::RoundingStrategy](docs/RoundingStrategy.md)
 - [SwaggerClient::Second](docs/Second.md)
 - [SwaggerClient::SiBaseUnit](docs/SiBaseUnit.md)
 - [SwaggerClient::SiBaseUnit1](docs/SiBaseUnit1.md)
 - [SwaggerClient::SiSystemOfUnits](docs/SiSystemOfUnits.md)
 - [SwaggerClient::SiSystemOfUnits1](docs/SiSystemOfUnits1.md)
 - [SwaggerClient::SystemOfUnits](docs/SystemOfUnits.md)
 - [SwaggerClient::SystemOfUnits1](docs/SystemOfUnits1.md)
 - [SwaggerClient::SystemOfUnits2](docs/SystemOfUnits2.md)
 - [SwaggerClient::SystemOfUnits3](docs/SystemOfUnits3.md)
 - [SwaggerClient::UnauthorizedError](docs/UnauthorizedError.md)
 - [SwaggerClient::Unit](docs/Unit.md)
 - [SwaggerClient::Unit1](docs/Unit1.md)
 - [SwaggerClient::WorkHour](docs/WorkHour.md)


## Documentation for Authorization

 All endpoints do not require authorization.
