FROM ansibleplaybookbundle/apb-base

LABEL "com.redhat.apb.version"="0.1.0"
LABEL "com.redhat.apb.spec"=\
"aWQ6IDk3NjI2MmQ4LWEyMzUtNGI4Yy1hYjAxLTBkNTEwNjg5YzVmNgpuYW1lOiBoZWxsby13b3Js\
ZC1hcGIKaW1hZ2U6IGFuc2libGVwbGF5Ym9va2J1bmRsZS9oZWxsby13b3JsZC1hcGIKZGVzY3Jp\
cHRpb246IGhlbGxvLXdvcmxkLWFwYiBkZXNjcmlwdGlvbgpiaW5kYWJsZTogRmFsc2UKYXN5bmM6\
IG9wdGlvbmFsCm1ldGFkYXRhOgogIGRpc3BsYXlOYW1lOiBIZWxsbyBXb3JsZCAoQVBCKQogIGxv\
bmdEZXNjcmlwdGlvbjogQSBzYW1wbGUgQVBCIHRvIGRlcGxveSBIZWxsbyBXb3JsZAogIGRlcGVu\
ZGVuY2llczogWydkb2NrZXIuaW8vYW5zaWJsZXBsYXlib29rYnVuZGxlL2hlbGxvLXdvcmxkOmxh\
dGVzdCddCnBsYW5zOgogIC0gbmFtZTogZGVmYXVsdAogICAgZGVzY3JpcHRpb246IEEgc2FtcGxl\
IEFQQiB3aGljaCBkZXBsb3lzIEhlbGxvIFdvcmxkCiAgICBmcmVlOiBUcnVlCiAgICBtZXRhZGF0\
YToKICAgICAgZGlzcGxheU5hbWU6IERlZmF1bHQKICAgICAgbG9uZ0Rlc2NyaXB0aW9uOiBUaGlz\
IHBsYW4gZGVwbG95cyBhIFB5dGhvbiB3ZWIgYXBwbGljYXRpb24gZGlzcGxheWluZyBIZWxsbyBX\
b3JsZAogICAgICBjb3N0OiAkMC4wMAogICAgcGFyYW1ldGVyczogW10K"
LABEL "io.openshift.tags"="apb"
architecture=x86_64
authoritative-source-url=registry.access.redhat.com
com.redhat.component=openshift-enterprise-helloworld-apb
distribution-scope=public
io.k8s.description=The Red Hat Enterprise Linux Base image is designed to be a fully supported foundation for your containerized applications. This base image provides your operations and application teams with the packages, language runtimes and tools necessary to run, maintain, and troubleshoot all of your applications. This image is maintained by Red Hat and updated regularly. It is designed and engineered to be the base layer for all of your containerized applications, middleware and utilites. When used as the source for all of your containers, only one copy will ever be downloaded and cached in your production environment. Use this image just like you would a regular Red Hat Enterprise Linux distribution. Tools like yum, gzip, and bash are provided by default. For further information on how this image was built look at the /root/anacanda-ks.cfg file.
io.k8s.display-name=Red Hat Enterprise Linux 7
release=7
summary=Provides the latest release of Red Hat Enterprise Linux 7 in a fully featured and supported base image.
url=https://access.redhat.com/containers/#/registry.access.redhat.com/openshift3/mediawiki-apb/images/v3.6.173.0.5-7
vcs-ref=c82284c028f6c484f3f138c797c661da05dbc748
vcs-type=git
vendor=Red Hat, Inc.
version=v3.6.173.0.5

ADD playbooks /opt/apb/actions
ADD roles /opt/ansible/roles
RUN chmod -R g=u /opt/{ansible,apb}

USER apb
