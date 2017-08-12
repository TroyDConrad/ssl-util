# ssl-util
Utility for generating CSRs, purchasing certificates and installing in Amazon AWS.

To install:

$ cd && rm -rf ssl-util && git clone https://github.com/TroyDConrad/ssl-util.git && cd ssl-util && sudo ./install.sh

For a fresh install, edit the /etc/ssl-util/settings.yml file and add the following:

# SSL certificate base directory
ssl_certificate_dir: <ssl certificate directory, usually '/etc/ssl_certificates'>

# AWS access credentials (used to upload cert to AWS IAM)
aws_access_key: <AWS access key>
aws_secret_key: <AWS secret key>

# CSR (Certificate Signing Request) settings
organization: <organization name>
department: <department name>
city: <city name>
state: <state name>
country_csr: <country name, e.g. 'US'>
email: <email address>
