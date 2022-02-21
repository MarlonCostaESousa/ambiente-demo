FROM webjump/magento2-php:7.4.8-alpine

USER www-data

RUN COMPOSER_MEMORY_LIMIT=-1 composer config --global http-basic.repo.magento.com 4ffe97e4a29cfdf4efb90d6b7468a632 679f6511d42b67bb66992f0375d8bd74 \
&& COMPOSER_MEMORY_LIMIT=-1  composer create-project --repository-url=https://repo.magento.com/ magento/project-enterprise-edition magento2
