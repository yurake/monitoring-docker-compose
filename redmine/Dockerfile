FROM redmine:10.4.7
# FROM redmine:3.4.11

RUN cd /usr/src/redmine/plugins \
    && git clone https://github.com/noshutdown-ru/redexporter.git \
    && chown -R redmine.redmine redexporter \ 
    && gem install vmstat -v '2.3.1' --source 'https://rubygems.org/' \
    && bundle install \
    && bundle exec rake redmine:plugins:migrate RAILS_ENV=production

