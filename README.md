## DESCRIPTION
Exhibitor is a supervisor system for ZooKeeper.

## DETAILS

Please see the doc at https://github.com/Netflix/exhibitor/wiki

## BUILDING

Exhibitor is built via Gradle (http://www.gradle.org). To build from the command line:
    ./gradlew build

### DEBIAN PACKAGE

To build the Debian package you need to have [FPM](https://github.com/jordansissel/fpm) installed.

    fpm -t deb -n exhibitor -v 1.5.6 --description "Zookeeper co-process" --category misc --vendor Netflix --url "https://github.com/Netflix/exhibitor" --after-install ./exhibitor.postinst --prefix=/ --config-files=/etc/exhibitor/log4j.properties --config-files=/etc/default/exhibitor --config-files=/etc/init/exhibitor.conf -s dir -C debian/ etc/ opt/ var/


## ARTIFACTS

Exhibitor binaries are published to Maven Central. Please see the docs for details.

## MAILING LIST

There is an Exhibitor mailing list. Join here: http://groups.google.com/group/exhibitor-users

## AUTHOR

Jordan Zimmerman (jordan@jordanzimmerman.com)

## LICENSE

Copyright 2012 Netflix, Inc.

Licensed under the Apache License, Version 2.0 (the “License”); you may not use this file except in
compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software distributed under the License is
distributed on an “AS IS” BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
implied. See the License for the specific language governing permissions and limitations under the
License.
