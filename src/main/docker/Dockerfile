FROM registry.access.redhat.com/ubi8/openjdk-17-runtime:1.19

ENV LANGUAGE='en_US:en'

# copy application bundle
COPY --chown=185 target/test-camel-balance-client*.jar /deployments/bundle.jar

EXPOSE 8080
USER 185

ENV JAVA_APP_JAR="/deployments/bundle.jar"

