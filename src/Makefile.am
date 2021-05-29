lib_LTLIBRARIES=libplugin_test.la libplugin_file.la

if PLUGIN_BUILD_MYSQL
lib_LTLIBRARIES += libplugin_mysql.la
libplugin_mysql_la_SOURCES=mysqlauth.c ../ext/cJSON.c common.c
libplugin_mysql_la_CFLAGS=-fPIC -I ../ext
libplugin_mysql_la_LDFLAGS= -shared -module -export-dynamic -version-info 1:0:0

endif

libplugin_test_la_SOURCES=testauth.c
libplugin_test_la_CFLAGS=-fPIC
libplugin_test_la_LDFLAGS= -shared -module -export-dynamic -version-info 1:0:0

libplugin_file_la_SOURCES=fileauth.c ../ext/cJSON.c common.c
libplugin_file_la_CFLAGS=-fPIC -I ../ext
libplugin_file_la_LDFLAGS= -shared -module -export-dynamic -version-info 1:0:0

