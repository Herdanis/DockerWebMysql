FROM php:7.4-fpm

# Install system dependencies
RUN apt-get update && apt-get install -y \
    git \
    curl \
    cron \
    cron \
    libpng-dev \
    libonig-dev \
    libxml2-dev \
    libfreetype6-dev \
    libicu-dev \
    libjpeg62-turbo-dev \
    libmcrypt-dev \
    libxslt1-dev \
    libzip-dev \
    zip \
    unzip

# Clear cache
RUN apt-get clean && rm -rf /var/lib/apt/lists/*

# Install PHP extensions
RUN docker-php-ext-install \
    bcmath \
    ctype \
    fileinfo \
    json \
    mbstring \
    pdo_mysql \
    tokenizer \
    xml \
    exif \
    pcntl \
    gd \
    intl \
    xsl \
    zip \
    soap

# Get latest Composer
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer