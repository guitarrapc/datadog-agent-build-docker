FROM datadog-build-base-official:1.0.0
WORKDIR $GOPATH/src/github.com/DataDog/datadog-agent
RUN git fetch origin master
RUN git checkout master
RUN git merge origin/master
RUN invoke agent.build --build-exclude=snmp,systemd
