# Trading Office - Market Data Service
[![Build Status](https://travis-ci.org/spolnik/trading-office-market-data-service.svg?branch=master)](https://travis-ci.org/spolnik/trading-office-market-data-service) [![codecov.io](https://codecov.io/github/spolnik/trading-office-market-data-service/coverage.svg?branch=master)](https://codecov.io/github/spolnik/trading-office-market-data-service?branch=master) [![Sonar Coverage](https://img.shields.io/sonar/https/sonar-nprogramming.rhcloud.com/trading-office-market-data-service/coverage.svg)](https://sonar-nprogramming.rhcloud.com/dashboard/index/1) [![Sonar Tech Debt](https://img.shields.io/sonar/https/sonar-nprogramming.rhcloud.com/trading-office-market-data-service/tech_debt.svg)](https://sonar-nprogramming.rhcloud.com/dashboard/index/1)

Trading Office is reference implementation of microservices architecture, based on Spring Boot. It's modeling part of post trade processing, mainly focused on receiving Fixml message and preparing confirmation for it.

- [Trading Office](#trading-office)
- [Market Data Service](#market-data-service)
- [Notes](#notes)

## Trading Office

- [Trading Office](https://github.com/spolnik/trading-office)

## Market Data Service
- spring boot web application
- exposes REST endpoint for market data (using Yahoo Finance Api)
- exposes REST endpoints for instrument data (data consumed from [OpenFigi Api](https://openfigi.com/api))
- based on a given symbol, downloads instrument data with actual price
- works in readonly mode

Heroku: http://market-data-service.herokuapp.com/swagger-ui.html

![Component Diagram](https://raw.githubusercontent.com/spolnik/trading-office-market-data-service/master/design/market_data_service.png)

## Notes
- checking if [dependencies are up to date](https://www.versioneye.com/user/projects/56ad39427e03c7003ba41427)