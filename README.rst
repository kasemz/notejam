*******
Notejam
*******

**Notejam deployed on  Azure platform**


Notejam Notejam is a Python/Flask monolith application. The document describes a proposed approach to migrate monolithic application to containers on Azure with CI/CD.

Architecture
This application in its originaly is built as a monolith having a stateless webserver and SQLite  both are running on the same VM or machine. 

**To Improve scalability, security and devlopment**

1- the database has been decoupled and replaced by an Azure SQL Database.
2- the application is packed to Docker image and sent Azure Container register to be deployed to Azure as Webapp container based more over how to deploy can be found on (https://docs.microsoft.com/en-us/azure/devops/pipelines/apps/cd/deploy-docker-webapp?view=azure-devops&tabs=java)
3- Azure Kubernetes is alos implemented to improve scalability
4- Monitoring is garanted by sending the logs to log Analytics workspace.
5- It is also possible to store connections strings and key certificates in an Azure Key Vault.
6- Implementing WAF ( Web application firewall) which acts as Load balancer and firewall, might improve security.


**Suggusted new architecture**































**The easy way to learn web frameworks**

Do you know framework X and want to try framework Y?
The easy way to start with a new framework is to compare it with frameworks you already know.
The goal of the project is to help developers easily learn new frameworks by examples.

Notejam is a unified sample web application (more than just "Hello World") implemented using different server-side frameworks.
Currently python, php, ruby and javascript frameworks are supported.


====================
Supported frameworks
====================

**Python**


* `Django <https://github.com/komarserjio/notejam/tree/master/django>`_
* `Flask <https://github.com/komarserjio/notejam/tree/master/flask>`_
* `Pyramid <https://github.com/komarserjio/notejam/tree/master/pyramid>`_

**PHP**

* `Laravel <https://github.com/komarserjio/notejam/tree/master/laravel>`_
* `Yii <https://github.com/komarserjio/notejam/tree/master/yii>`_
* `CakePHP <https://github.com/komarserjio/notejam/tree/master/cakephp>`_
* `Nette <https://github.com/komarserjio/notejam/tree/master/nette/native_db>`_ / `Nette + Doctrine <https://github.com/komarserjio/notejam/tree/master/nette/doctrine>`_
* `Symfony <https://github.com/komarserjio/notejam/tree/master/symfony>`_

**Ruby**

* `Padrino <https://github.com/komarserjio/notejam/tree/master/padrino>`_
* `Ruby on Rails <https://github.com/komarserjio/notejam/tree/master/rubyonrails>`_

**Java**

* `Spring <https://github.com/komarserjio/notejam/tree/master/spring>`_

**Javascript (node.js)**

* `Express <https://github.com/komarserjio/notejam/tree/master/express>`_


In progress
-----------

**Scala**

* Play

**Clojure**

* Compojure

... and more frameworks are coming soon.

====================
Application overview
====================

Notejam is a web application which offers user to sign up/in/out and create/view/edit/delete notes.
Notes are grouped in pads.

**Screenshots**

.. image:: https://github.com/komarserjio/notejam/blob/master/html/screenshots/1p.png
    :alt: Sign in
    :width: 400
    :align: center
    :target: https://github.com/komarserjio/notejam/tree/master/screenshots.rst

.. image:: https://github.com/komarserjio/notejam/blob/master/html/screenshots/2p.png
    :alt: All notes
    :width: 400
    :align: center
    :target: https://github.com/komarserjio/notejam/tree/master/screenshots.rst

.. image:: https://github.com/komarserjio/notejam/blob/master/html/screenshots/3p.png
    :alt: New note
    :width: 400
    :align: center
    :target: https://github.com/komarserjio/notejam/tree/master/screenshots.rst

See `more screenshots <https://github.com/komarserjio/notejam/tree/master/screenshots.rst>`_
for look and feel.

See `detailed overview <https://github.com/komarserjio/notejam/blob/master/contribute.rst#application-requirements>`_.

Typical application covers following topics:

* Request/Response handling
* Routing
* Templates
* Configuration
* Authentication
* Forms
* Error handling
* Database/ORM
* Mailing
* Functional/unit testing

=============
How to launch
=============

All implementations are SQLite based and quickly launchable by built-in web servers.
Each implementation has instruction describing easy steps to install environment, launch and run tests.

============
Contribution
============

Contribution is more than welcome!
Contribute improvements to existing applications to help them follow best practices
or provide new implementation for unsupported framework.


**Do you want to improve one of the existing implementations?**

Each implementation has its own README with contribution details.

**Do you want to add new framework?**

Read `contribution guide <https://github.com/komarserjio/notejam/blob/master/contribute.rst>`_ for details.

========
Contacts
========

* Twitter: `@komarserjio <https://twitter.com/komarserjio>`_
* Email: komarserjio <at> gmail.com

=======
License
=======

MIT © Serhii Komar.

See `license <https://github.com/komarserjio/notejam/blob/master/license.rst>`_.
