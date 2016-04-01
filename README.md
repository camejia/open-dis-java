# open-dis-java
Open-DIS git repository for the Java implementation

[![Build Status](https://travis-ci.org/open-dis/open-dis-java.svg?branch=master)](https://travis-ci.org/open-dis/open-dis-java)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/edu.nps.moves/open-dis/badge.svg)](https://maven-badges.herokuapp.com/maven-central/edu.nps.moves/open-dis)

## Software release process

Once enough changes have been made we cut a new release and deploy it to Maven Central.

In a nutshell the person performing the release will need:
 * A Sonatype JIRA account
 * Your JIRA credentials placed in your `~/.m2/settings.xml`
 * Your GPG key published

For more info view this [guide](https://docs.sonatype.org/display/Repository/Sonatype+OSS+Maven+Repository+Usage+Guide).

Once that's done, for each release do the following commands:

    $ mvn release:clean
    $ mvn release:prepare
    $ mvn release:perform
