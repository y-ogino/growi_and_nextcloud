FROM nextcloud:apache

# The Nextcloud Docker image does not install the package 'smbclient',
# without which the 'SMB / CIFS' option in the 'External storage support' app is not available.
# Refer to https://github.com/docker-library/owncloud/pull/79
RUN  apt-get update -y && apt-get install -y smbclient