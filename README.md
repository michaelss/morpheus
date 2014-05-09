Morpheus
========

JSON x SQL mapper enhanced.

Morpheus main objective is to boost the development of not so complex applications by allowing some metadata in the URLs.

## Premises

To adopt Morpheus in its first version, applications must meet the following technical requirements:

* Use relational databases
* Be REST based
* Adopt JSON as transfer format


## Principles

* By "not so complex applications", I mean the vast majority of applications. This includes CRUDs (with one table and at least one level relationships), CMSs, plain listings, listings with sublevels (including master-details), listings with filters.

* Metadata in the URLs include columns, conditions, relationships, sorting and grouping. Table names will not be exposed on the URL's.

* Morpheus will translate the URL metadata into SQL commands, execute them and format and return the results as JSON objects and arrays.

* Returning JSONs may be transformed on the server side with JavaScript (Node.js or Nashorn) before being sent to the client. The transformation scripts will be indicated in the URL too.

* Morpheus will provide a login window and an authorization mechanism based on systems and roles (RBAC - Role Based Access Control).

* Further work in this project may include the creation of adherent front-end templates with JavaScript MVC framework (I tend to use Angular or Ember).