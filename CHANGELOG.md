# Change Log

## 0.3.2 - 2016-05-06

* Removed `sonarqube` profile and Sonarqube related properties because every project may configure it a little differently.
* Set `quiet=true` to maven-javadoc-plugin to reduce printout on the log.

## 0.3.1 - 2016-05-04

* `sonarqube` profile to fix SonarQube's 5.x "Class Not Found" errors.

## 0.3.0 - 2016-04-29

* Minimum Java version is 7.
* Removed `java6` profile.

* Plugin updates.

```text
maven-project-info-reports-plugin ...................... 2.8.1 -> 2.9
maven-site-plugin ...................................... 3.4 -> 3.5.1
maven-source-plugin .................................... 2.4 -> 3.0.0
org.jacoco:jacoco-maven-plugin  0.7.5.201505241946 -> 0.7.6.201602180812
org.sonarsource.scanner.maven:sonar-maven-plugin ..... 3.0.1 -> 3.0.2
org.sonatype.plugins:nexus-staging-maven-plugin ...... 1.6.6 -> 1.6.7
```

## 0.2.4 - 2016-01-20

* Plugin updates.

```text
org.jacoco:jacoco-maven-plugin  0.7.4.201502262128 -> 0.7.5.201505241946
```

* Configured to work with Sonar 5.x.
* Renamed profile `external-release` to `ossrh-deploy`.

## 0.2.3 - 2016-01-13

* Compatible with Java 7 and 8. 
* Add `-P java6` use it with Java 6. The `java6` profile will be removed in the near future.
* Add `versions-maven-plugin` to make it easier to upgrade plugins.
* Plugin updates.

```text
maven-failsafe-plugin .............................. 2.18.1 -> 2.19.1
maven-pmd-plugin ......................................... 3.5 -> 3.6
maven-project-info-reports-plugin ...................... 2.8 -> 2.8.1
maven-surefire-plugin .............................. 2.18.1 -> 2.19.1
maven-surefire-report-plugin ....................... 2.18.1 -> 2.19.1
org.codehaus.mojo:findbugs-maven-plugin .............. 2.5.5 -> 3.0.3
org.sonatype.plugins:nexus-staging-maven-plugin ...... 1.6.5 -> 1.6.6
```

## 0.2.2 - 2015-09-15

* Downgrade JaCoCo from 0.7.5.201505241946 to 0.7.4.201502262128 because the coverage reports won't show up in Jenkins.
            
## 0.2.1 - 2015-07-23

* Enable `noJekyll` option in GitHub Site Plugin to allow JaCoCo web reports to show up properly in GitHub pages.

## 0.2.0 - 2015-07-23

* Attach `site:attach-descriptor` in Maven Site Plugin to allow Maven 3 to pick up `src/site/site.xml`.

## 0.1.0 - 2015-07-22

* Initial.
