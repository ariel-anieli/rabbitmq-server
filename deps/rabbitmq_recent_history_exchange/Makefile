PROJECT = rabbitmq_recent_history_exchange
PROJECT_DESCRIPTION = RabbitMQ Recent History Exchange

define PROJECT_APP_EXTRA_KEYS
	{broker_version_requirements, []}
endef

DEPS = rabbit_common rabbit khepri khepri_mnesia_migration
TEST_DEPS = rabbitmq_ct_helpers rabbitmq_ct_client_helpers amqp_client

PLT_APPS += mnesia

DEP_EARLY_PLUGINS = rabbit_common/mk/rabbitmq-early-plugin.mk
DEP_PLUGINS = rabbit_common/mk/rabbitmq-plugin.mk

include ../../rabbitmq-components.mk
include ../../erlang.mk
