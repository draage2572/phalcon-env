# Pull base image
FROM phalconphp/php:7

MAINTAINER Adrian Eavaz <adrian.eavaz@gmail.com>

# Set environment variables
ADD http://codeception.com/codecept.phar /usr/local/bin/codecept
RUN chmod +x /usr/local/bin/codecept

# Display version information
RUN codecept --version

# Set up the application directory
VOLUME ["/app"]

# Define working directory
WORKDIR /application

# Set up the command arguments
CMD ["-"]
ENTRYPOINT ["codecept"]