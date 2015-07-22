# newrelic-s3-context
Pump S3 metrics into New Relic with Context on the contents of the bucket.

Full credit to https://github.com/adstage/newrelic_s3_plugin.  The code started there, but I didn't fork because its going a completely different direction.

## Install

1. git clone https://github.com/MNiedzielski/newrelic-s3-context.git
2. Edit `config/newrelic_plugin.yml`
      a. replace "YOUR_LICENSE_KEY_HERE" with your New Relic license key
      b. replace AWS credentials with your credentials
      c. Copy bucket config and put in bucket region and name for each bucket you want to monitor
3. bundle install
4. bundle exec daemon start

For bonus points run under supervision. We recommend monit.
