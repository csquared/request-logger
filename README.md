# Request Logger

this is demo add-on that shows how one could log and modify an HTTP request
before it hits a Heroku application.

# Installation

it expects the user to install my rack-cgi-proxy and configure it via:

  Gemfile:

    gem 'rack-cgi-proxy', :git => 'git://github.com/csquared/rack-cgi-proxy.git'

  config.ru

    use Rack::CgiProxy, ENV['REQUEST_LOGGER_URL']

  Install Add-on

    heroku addons:add request-logger
