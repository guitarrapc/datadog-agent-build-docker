FROM datadog-build-base-official:1.0.0
WORKDIR $GOPATH/src/github.com/DataDog/datadog-agent
RUN invoke agent.build --build-exclude=snmp,systemd
