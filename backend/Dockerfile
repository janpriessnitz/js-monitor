FROM openshift-registry.web.cern.ch/openshift/nodejs:10

USER root

# TODO: uncomment as soon as libcvmfs built with -fPIC is released
#RUN yum install -y https://ecsft.cern.ch/dist/cvmfs/cvmfs-release/cvmfs-release-latest.noarch.rpm
#RUN yum install -y cvmfs-devel

RUN yum install -y curl
RUN curl http://ecsft.cern.ch/dist/cvmfs/nightlies/cvmfs-git--2187/cvmfs-devel-2.8.0-0.2187.fabc685f4faff38fgit.el7.x86_64.rpm > /root/cvmfs-devel.rpm
RUN rpm -i /root/cvmfs-devel.rpm


USER 1001
