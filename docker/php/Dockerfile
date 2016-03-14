FROM php:7-fpm

RUN apt-get update
RUN apt-get install -y libcurl4-gnutls-dev libxml2-dev libbz2-dev libpng++-dev \
    libpng3 libjpeg-dev libvpx-dev zlib1g-dev libgd-dev libssl-dev \
    libtidy-dev libxslt1-dev libmagic-dev libexif-dev file curl wget

RUN pecl install apcu
RUN pecl install xdebug
RUN docker-php-ext-install curl dom bz2 gd json mysqli pcntl pdo pdo_mysql phar posix
RUN docker-php-ext-install simplexml soap tidy tokenizer xml
RUN docker-php-ext-install xmlwriter xsl zip bcmath calendar ctype
RUN docker-php-ext-install exif
RUN docker-php-ext-install fileinfo
