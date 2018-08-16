Changelog
---------

0.7.4 (2018-08-15)
~~~~~~~~~~~~~~~~~~
* fix #33 error when nothing to resume using --resume

0.7.3 (2018-08-14)
~~~~~~~~~~~~~~~~~~
* fix #31 es_update movies --newer --workers does not store worker information

0.7.2 (2018-08-13)
~~~~~~~~~~~~~~~~~~
* fix #21 wrong batch update total using multiprocessing in 0.7.1
* fix #23 KeyError _index_version_name in es_update --newer
* address #25 use pks for queryset inside workers #29

0.7.1 (2018-08-07)
~~~~~~~~~~~~~~~~~~
* fixed gh #8 es_dangerous_reset --es-only to sync database to ES
* fixed gh #17 make es_dangerous_reset remove dem models
* improved test coverage
* added tests for ``es_create --es-only``
* added ``IndexVersion.hard_delete()`` (not called by default)
* added ``hard_delete`` flag to ``DropIndexAction``
* added ``hard_delete`` flag to ``DEMIndexManager.test_post_teardown()``
* updated ``__str__()`` of ``IndexAction`` to be more descriptive

0.7.0 (2018-08-06)
~~~~~~~~~~~~~~~~~~
* fixed gh #5: "add python 3 support and tests"

0.6.1 (2018-08-03)
~~~~~~~~~~~~~~~~~~
* fixed gh #9: "using elasticsearch-dsl 6.1, TypeError in DEMIndex.save"

0.6.0 (2018-08-01)
~~~~~~~~~~~~~~~~~~
* Added test structure for py2 - GH #2
* Renamed default log handler from ``django-elastic-migrations`` to ``django_elastic_migrations``

0.5.3 (2018-07-23)
~~~~~~~~~~~~~~~~~~
* First basic release