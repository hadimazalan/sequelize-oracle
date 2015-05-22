# Sequelize-oracle
  
[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/lebretr/sequelize-oracle/trend.png)](https://bitdeli.com/free "Bitdeli Badge") 
[![Build Status](https://travis-ci.org/lebretr/sequelize-oracle.svg?branch=master-Oracle-dev)](https://travis-ci.org/lebretr/sequelize-oracle) 
[![Dependency Status](https://david-dm.org/lebretr/sequelize-oracle.png)](https://david-dm.org/lebretr/sequelize-oracle) 
[![Code Climate](https://codeclimate.com/github/lebretr/sequelize-oracle/badges/gpa.svg)](https://codeclimate.com/github/lebretr/sequelize-oracle) 
[![Test Coverage](https://codeclimate.com/github/lebretr/sequelize-oracle/badges/coverage.svg)](https://codeclimate.com/github/lebretr/sequelize-oracle)

Sequelize is a promise-based Node.js/io.js ORM for Postgres, MySQL, MariaDB, SQLite, Microsoft SQL Server and Oracle. It features solid transaction support, relations, read replication and more.

### Note
sequelize-oracle is a fork of [sequelize@master](https://github.com/sequelize/sequelize/tree/master) 
this fork add support of DML statements for Oracle  
If you don't need Oracle support, prefer the original [Sequelize](http://sequelizejs.com/)  
  
Sequelize-oracle@3.x.x-x.x is in development. Only the old version (1.10.x-x.x) is on npmjs registry.  

## Compatibility:
Sequelize-oracle is compatible only with nodejs@0.10.x (oracledb limitation).  
Sequelize-oracle is only tested with Oracle 11 XE.  
  
## Installation

```
npm install oracledb
npm install sequelize
```

## Limitations:

- DataType: only this dataTypes are managed: 
  - STRING (=VARCHAR2)
  - CHAR
  - DECIMAL (=NUMBER)
  - BIGINT (=NUMBER(19,0))
  - INTEGER
  - FLOAT 
  - DOUBLE
  - UUID (=CHAR 36)
  - DATE (=TIMESTAMP WITH LOCAL TIME ZONE)
  - DATEONLY (=DATETIME) 
  - BOOLEAN (=NUMBER(1))
- Index: index type is not fully managed
  
## Todo:
- ENUM DataType
- improve index for type
- RETURNING in update and insert query
- resolve the pb "name column length > 30 char" in nesteed querry
- ...
  
  
  
# Sequelize

[![Build Status](https://travis-ci.org/sequelize/sequelize.svg?branch=master)](https://travis-ci.org/sequelize/sequelize) [![Dependency Status](https://david-dm.org/sequelize/sequelize.svg)](https://david-dm.org/sequelize/sequelize) [![Test Coverage](https://codeclimate.com/github/sequelize/sequelize/badges/coverage.svg)](https://codeclimate.com/github/sequelize/sequelize)
[![Bountysource](https://www.bountysource.com/badge/team?team_id=955&style=bounties_received)](https://www.bountysource.com/teams/sequelize/issues?utm_source=Sequelize&utm_medium=shield&utm_campaign=bounties_received)
[![Flattr this](http://api.flattr.com/button/flattr-badge-large.png)](http://flattr.com/thing/1259407/Sequelize)

Sequelize is a promise-based Node.js/io.js ORM for Postgres, MySQL, MariaDB, SQLite and Microsoft SQL Server. It features solid transaction support, relations, read replication and more.

[Documentation](http://sequelize.readthedocs.org/en/latest/)

## Installation

`npm install sequelize`

From 3.0.0 and up Sequelize will follow SEMVER. 3.0.0 contains important security fixes so we highly recommend that users upgrade.

If you still use 1.7 please prefer to [Upgrading to 2.0](https://github.com/sequelize/sequelize/wiki/Upgrading-to-2.0) and the changelog between 2.0 and 3.0. 2.1 also has a breaking change.

## Features

- Schema definition
- Schema synchronization/dropping
- 1:1, 1:M & N:M Associations
- Through models
- Promises
- Hooks/callbacks/lifecycle events
- Prefetching/association including
- Transactions
- Migrations
- CLI ([sequelize-cli](https://github.com/sequelize/cli))

## Resources
- [Changelog](https://github.com/sequelize/sequelize/blob/master/changelog.md)
- [Getting Started](http://docs.sequelizejs.com/en/latest/docs/getting-started/)
- [Documentation](http://docs.sequelizejs.com/en/latest/)
- [API Reference](http://docs.sequelizejs.com/en/latest/)
- [Collaboration and pull requests](https://github.com/sequelize/sequelize/blob/master/CONTRIBUTING.md)
- [Roadmap](https://github.com/sequelize/sequelize/issues/2869)
- [Twitter](https://twitter.com/SequelizeJS): @SequelizeJS
- [IRC](http://webchat.freenode.net?channels=sequelizejs): sequelizejs on Freenode
- [Google Groups](https://groups.google.com/forum/#!forum/sequelize)
- [Add-ons & Plugins](https://github.com/sequelize/sequelize/wiki/Add-ons-&-Plugins)
