# zipcache
Public repo, docs, website for ZipCache.com
Kodiak S3Proxy/Edgecache
How to build Kodiak-S3
CentOS X86_64 platform
Preparation
Any CentOS 7 platform
git clone https://github.com/kodiakdata/Kodiak-S3.git
node and node-gyp are pointing to the correct version
Current nodejs version for x86_64 is 8.9.0
Build RPM
make build_rpm
KodiakS3Proxy RPM will be under /root/rpmbuild/RPMS/x86_64
Debian X86_64 platform
Preparation Same as CentOS x86_64 above

Build Debian package

Any Debian platform
make build_dpkg DEBIAN=1
Debian package will be under directory build-debian/KodiakS3Proxy
Debian armv7l platform
Preparation
Any Debian armv7l ODroid
git clone https://github.com/kodiakdata/Kodiak-S3.git
Path for node and node-gyp are pointing to the correct version
Current nodejs version for armv7l is 8.9.4
Build Debian package
 make build_dpkg DEBIAN=1
Debian package will be under build-debian/KodiakS3Proxy
Docker image for x86_64 platform
Preparation
Any x86_64 running Docker CE
git clone https://github.com/kodiakdata/Kodiak-S3.git
Path for node and node-gyp are pointing to the correct version
Current nodejs version for x86_64 docker image is 8.9.4
Build Docker image for x86_64
make docker_image
Docker image kodiakdata/edgecache:latest will be under 'docker images'
Docker image for armv7l platform
Preparation
Any Debian armv7l ODroid
git clone https://github.com/kodiakdata/Kodiak-S3.git
Path for node and node-gyp are pointing to the correct version
Current nodejs version for armv7l docker image is 8.9.4
Build Docker image for armv7l
make docker_image DEBIAN=1
Docker image kodiakdata/edgecache:armv7l will be under 'docker images'
How to run Kodiak-S3
CentOS x86_64
Install
rpm -I KodiakS3Proxy-<version>.rpm
Update
rpm -U KodiakS3Proxy-<version>.rpm
Debian x86_64
Install
dpkg -i KodiakS3Proxy-<version>.deb
Update
dpkg -u KodiakS3Proxy-<version>.deb
Docker
Install
Instructions on running in Docker
