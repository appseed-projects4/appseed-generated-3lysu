# Change Log

## [0.0.22] 2024-09-02
### Changes

- Added Interactive Generator 
  - The Output JSON can be used later to generate a Django starter 
```bash
$ python manage.py tool_generator_interactive -i # Print HELP 
$ python manage.py tool_generator_interactive    # Generate JSON File  
```

## [0.0.21] 2024-09-01
### Changes

- Added DB Processor
  - Supports DB introspection for data and tables definition: SQLite, Mysql, PGSQL
- Added CSV Processor
  - Local, Remote versions
  - CSV to Django Model
- DOCS: [CSV Processor](https://app-generator.dev/docs/developer-tools/csv-processor.html)
  
```bash
> Processing .\media\tool_inspect\csv_inspect_distant.json
    |-- file: https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv
    |-- type: csv

Field        CSV Type    Django Types
-----------  ----------  ------------------------------------------
PassengerId  int64       models.IntegerField(blank=True, null=True)
Survived     int64       models.IntegerField(blank=True, null=True)
Pclass       int64       models.IntegerField(blank=True, null=True)
Name         object      models.TextField(blank=True, null=True)
Sex          object      models.TextField(blank=True, null=True)
Age          float64     models.FloatField(blank=True, null=True)
SibSp        int64       models.IntegerField(blank=True, null=True)
Parch        int64       models.IntegerField(blank=True, null=True)
Ticket       object      models.TextField(blank=True, null=True)
Fare         float64     models.FloatField(blank=True, null=True)
Cabin        object      models.TextField(blank=True, null=True)
Embarked     object      models.TextField(blank=True, null=True)
```

## [0.0.20] 2024-08-07
### Changes

- Update Blog
  - Added Dynamic SEO: aticles & search
- Added [Bash](https://app-generator.dev/docs/technologies/bash.html) Node in DOCS
  - [Getting Started with Bash](https://app-generator.dev/docs/technologies/bash/index.html)
  - [Bash in Docker Scripts](https://app-generator.dev/docs/technologies/bash/docker.html)    

## [0.0.19] 2024-08-07
### Changes

- New [DOCS](https://app-generator.dev/docs/) Sections
  - [Developer Tools](https://app-generator.dev/docs/developer-tools.html)
    - [DataTables](https://app-generator.dev/docs/developer-tools/datatables.html)
    - [Dynamic DataTables](https://app-generator.dev/docs/developer-tools/dynamic-datatables.html)
    - [Dynamic API](https://app-generator.dev/docs/developer-tools/dynamic-api.html)
  - [Programming Concepts](https://app-generator.dev/docs/concepts.html)
    - [Metaprogramming](https://app-generator.dev/docs/concepts/metaprogramming.html)
    - [Aspect-Oriented Programming](https://app-generator.dev/docs/concepts/aspect-oriented-programming.html)
    - [Continuous Integration](https://app-generator.dev/docs/concepts/ci-cd.html)
    - [Concurrency and Parallelism](https://app-generator.dev/docs/concepts/concurrency.html)
    - [Design Patterns](https://app-generator.dev/docs/concepts/design-patterns.html)
    - [Domain-Driven Design](https://app-generator.dev/docs/concepts/domain-driven-design.html)
    - [Functional Programming](https://app-generator.dev/docs/concepts/functional-programming.html)
    - [Microservices Architecture](https://app-generator.dev/docs/concepts/microservices.html)
    - [N-Tier Architecture](https://app-generator.dev/docs/concepts/n-tier-architecture.html)
    - [Reactive Programming](https://app-generator.dev/docs/concepts/reactive-programming.html)

## [0.0.18] 2024-08-07
### Changes

- DOCS Update
  - [Flask](https://app-generator.dev/docs/technologies/flask.html) & [Getting Started Guide](https://app-generator.dev/docs/technologies/flask/index.html)
  - [Django](https://app-generator.dev/docs/technologies/django.html) & [Getting Started Guide](https://app-generator.dev/docs/technologies/django/index.html)

## [0.0.17] 2024-08-05
### Changes

- Refactor DOCS Section

## [0.0.16] 2024-07-30
### Changes

- HOMEpage Update (minor)

## [0.0.15] 2024-07-30
### Changes

- [AI Processor](https://app-generator.dev/ai-processor/)
- Enhance products
  - tags
  - videos 

## [0.0.14] 2024-06-19
### Changes

- Update OAuth Scope
  - Remove access to REPOs
  - Workflow
- Add CSV Processor (not fully tested)    

## [0.0.13] 2024-06-17
### Changes

- Update CLI: 
  - Added GitHub Uploader
- Django Core Template
  - Update README & Settings

## [0.0.12] 2024-06-16
### Changes

- Added Django generator
  - `$ python manage.py generator -f sources/input-template-volt.json`
- Update README

## [0.0.11] 2024-05-22
### Changes

- Integrate DOCS [ Sphinx ]

## [0.0.10] 2024-05-21
### Changes

- Refactor Codebase
  - Move [Util](https://github.com/app-generator/appseed-v2/tree/main/util) from apps -> ROOT 
- Added [Util.Logger](https://github.com/app-generator/appseed-v2/blob/main/util/logger/__init__.py)
  - Usage: Apps.Pages, `index()`
    - https://github.com/app-generator/appseed-v2/blob/main/apps/pages/views.py

Sample Output, that prints the TimeStamp, File, Function & Line Number

```log
2024-05-21 22:19:16.741500 - AppSeed, DEBUG [apps.pages.views->support(), L:23] Begin
```

## [0.0.9] 2024-05-21
### Changes

- Added Blog Section 
- Added DOCS Section
- Update GitHub Login Scope
  - Email
  - Repo access (private & public)
  - Workflow (CI/CD)

## [0.0.8] 2024-05-20
### Changes

- Added Celery Beat:
  - [CRON Settings](https://github.com/app-generator/appseed-v2/blob/main/core/celery.py)
  - [Tasks/Scripts](https://github.com/app-generator/appseed-v2/tree/main/tasks_scripts) DIR
  - [Tasks LOGS](https://github.com/app-generator/appseed-v2/tree/main/tasks_scripts/logs)
    - [Sample LOG](https://github.com/app-generator/appseed-v2/blob/main/tasks_scripts/logs/2024-05-20-16-30-critical_task.log)

## [0.0.7] 2024-05-20
### Changes

- Update HOMEpage
- Added new pages
  - Terms, About and Support 

## [0.0.6] 2024-05-19
### Changes

- Update `AppSeed V2` SPECS: 
  - [SPECS API](https://github.com/app-generator/appseed-v2/blob/main/apps/api/README.md)
  - [SPECS Auth](https://github.com/app-generator/appseed-v2/blob/main/apps/auth/README.md)
  - [SPECS Blog](https://github.com/app-generator/appseed-v2/blob/main/apps/blog/README.md)
  - [SPECS Deploy](https://github.com/app-generator/appseed-v2/blob/main/apps/deploy/README.md)
  - [SPECS Docs](https://github.com/app-generator/appseed-v2/blob/main/apps/docs/README.md)
  - [SPECS Generator](https://github.com/app-generator/appseed-v2/blob/main/apps/generator/README.md)
  - [SPECS Pages](https://github.com/app-generator/appseed-v2/blob/main/apps/pages/README.md)
  - [SPECS Products](https://github.com/app-generator/appseed-v2/blob/main/apps/products/README.md)
  - [SPECS Tasks](https://github.com/app-generator/appseed-v2/blob/main/apps/tasks/README.md)
  - [SPECS DevTools](https://github.com/app-generator/appseed-v2/blob/main/apps/tools/README.md)

## [0.0.5] 2024-05-19
### Changes

- Refactoring
- Added [CLI](https://github.com/app-generator/appseed-v2/tree/main/cli) & [Custom Commands](https://github.com/app-generator/appseed-v2/tree/main/cli/management):
  - `python manage.py help`         # Check the `CLI` app
  - `python manage.py cmd_apps`     # [Django - List all registered APPS](https://github.com/app-generator/appseed-v2/blob/main/cli/management/commands/cmd_apps.py) 
  - `python manage.py cmd_models`   # [Django - List models (app APPS)](https://github.com/app-generator/appseed-v2/blob/main/cli/management/commands/cmd_models.py)
  - `python manage.py cmd_showcfg`  # [Django - Print Configuration](https://github.com/app-generator/appseed-v2/blob/main/cli/management/commands/cmd_showcfg.py)

## [0.0.4] 2024-05-19
### Changes

- Added [LIVE Deploy](https://appseed-v2.onrender.com/) via Render
- Added SPECS for all apps:
  - [SPECS API](https://github.com/app-generator/appseed-v2/blob/main/apps/api/README.md)
  - [SPECS Aut](https://github.com/app-generator/appseed-v2/blob/main/apps/auth/README.md)
  - [SPECS Blog](https://github.com/app-generator/appseed-v2/blob/main/apps/blog/README.md)
  - [SPECS Deploy](https://github.com/app-generator/appseed-v2/blob/main/apps/deploy/README.md)
  - [SPECS Docs](https://github.com/app-generator/appseed-v2/blob/main/apps/docs/README.md)
  - [SPECS Generato](https://github.com/app-generator/appseed-v2/blob/main/apps/generator/README.md)
  - [SPECS Pages](https://github.com/app-generator/appseed-v2/blob/main/apps/pages/README.md)
  - [SPECS Products](https://github.com/app-generator/appseed-v2/blob/main/apps/products/README.md)
  - [SPECS Tasks](https://github.com/app-generator/appseed-v2/blob/main/apps/tasks/README.md)
  - [SPECS DevTools](https://github.com/app-generator/appseed-v2/blob/main/apps/tools/README.md)

## [0.0.3] 2024-05-18
### Changes

- Added APPS folders
  - mostly codebase structure changes 

## [0.0.2] 2024-05-10
### Changes

- Update RM (minor)

## [0.0.1] 2024-05-10
### Changes

- REPO Created
