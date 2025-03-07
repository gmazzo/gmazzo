# Guillermo Mazzola [![LinkedIn Profile](https://img.shields.io/badge/-gmazzo-0d65c2?logo=linkedin)](https://www.linkedin.com/in/gmazzo/)
[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=gmazzo&theme=onedark&count_private=true&hide_title=true&show_icons=true)](https://github.com/anuraghazra/github-readme-stats)

## Open Source projects

### JVM libraries
- [`okhttp-client-mock`](https://github.com/gmazzo/okhttp-client-mock)

  A simple `OKHttp` client mock, using a programmable request interceptor

  [![Stars](https://img.shields.io/github/stars/gmazzo/okhttp-client-mock)](https://github.com/gmazzo/okhttp-client-mock/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/okhttp-client-mock)](https://github.com/gmazzo/okhttp-client-mock/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/okhttp-client-mock)](https://github.com/gmazzo/okhttp-client-mock/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/okhttp-client-mock)](https://github.com/gmazzo/okhttp-client-mock/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/okhttp-client-mock)
  [![Maven Central](https://img.shields.io/maven-central/v/com.github.gmazzo.okhttp.mock/mock-client)](https://central.sonatype.com/artifact/com.github.gmazzo.okhttp.mock/mock-client)
  [![Build Status](https://github.com/gmazzo/okhttp-client-mock/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/okhttp-client-mock/actions/workflows/build.yaml)
  [![codecov](https://codecov.io/gh/gmazzo/okhttp-client-mock/branch/master/graph/badge.svg)](https://codecov.io/gh/gmazzo/okhttp-client-mock)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:okhttp-mock\b+content:com.github.gmazzo.okhttp+-repo:github.com/gmazzo/okhttp-client-mock&patternType=regexp)

  [![Contributors](https://contrib.rocks/image?repo=gmazzo/okhttp-client-mock)](https://github.com/gmazzo/okhttp-client-mock/graphs/contributors)

  ```kotlin
  val interceptor = MockInterceptor()
  
  interceptor.rule(url eq "https://testserver/api/json") {
    respond("{succeed:true}", MEDIATYPE_JSON)
  }
  ```

### Gradle plugins
- [`gradle-buildconfig-plugin`](https://github.com/gmazzo/gradle-buildconfig-plugin)

  A plugin for generating BuildConstants for any kind of Gradle projects: Java, Kotlin, Groovy, etc. Designed for KTS scripts.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-buildconfig-plugin)](https://github.com/gmazzo/gradle-buildconfig-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-buildconfig-plugin)](https://github.com/gmazzo/gradle-buildconfig-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-buildconfig-plugin)](https://github.com/gmazzo/gradle-buildconfig-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-buildconfig-plugin)](https://github.com/gmazzo/gradle-buildconfig-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-buildconfig-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/com.github.gmazzo.buildconfig)](https://plugins.gradle.org/plugin/com.github.gmazzo.buildconfig)
  [![Build Status](https://github.com/gmazzo/gradle-buildconfig-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-buildconfig-plugin/actions/workflows/build.yaml)
  [![codecov](https://codecov.io/gh/gmazzo/gradle-buildconfig-plugin/branch/master/graph/badge.svg)](https://codecov.io/gh/gmazzo/gradle-buildconfig-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:com.github.gmazzo.buildconfig+-repo:github.com/gmazzo/gradle-buildconfig-plugin)

  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-buildconfig-plugin)](https://github.com/gmazzo/gradle-buildconfig-plugin/graphs/contributors)

  ```kotlin
  buildConfig {
    buildConfigField("APP_NAME", project.name)
    buildConfigField("APP_VERSION", provider { "${project.version}" })
  ```
  
- [`gradle-android-test-aggregation-plugin`](https://github.com/gmazzo/gradle-android-test-aggregation-plugin)

  A couple Gradle plugins to make Android modules to work with [JaCoCo Report Aggregation Plugin](https://docs.gradle.org/current/userguide/jacoco_report_aggregation_plugin.html) and [Test Report Aggregation Plugin](https://docs.gradle.org/current/userguide/test_report_aggregation_plugin.html)

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-android-test-aggregation-plugin)](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-android-test-aggregation-plugin)](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-android-test-aggregation-plugin)](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-android-test-aggregation-plugin)](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-android-test-aggregation-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.test.aggregation.coverage)](https://plugins.gradle.org/plugin/io.github.gmazzo.test.aggregation.coverage)
  [![Build Status](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-android-test-aggregation-plugin/branch/main/graph/badge.svg?token=D5cDiPWvcS)](https://codecov.io/gh/gmazzo/gradle-android-test-aggregation-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.test.aggregation+-repo:github.com/gmazzo/gradle-android-test-aggregation-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-android-test-aggregation-plugin)](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/graphs/contributors)

  ![aggregated-jacoco-report](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/raw/main/README-aggregated-jacoco-report.png)
  
- [`gradle-testkit-jacoco-plugin`](https://github.com/gmazzo/gradle-testkit-jacoco-plugin)

  A Gradle plugin that enables JaCoCo coverage collection for Gradle TestKit's GradleRunner tests.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-testkit-jacoco-plugin)](https://github.com/gmazzo/gradle-testkit-jacoco-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-testkit-jacoco-plugin)](https://github.com/gmazzo/gradle-testkit-jacoco-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-testkit-jacoco-plugin)](https://github.com/gmazzo/gradle-testkit-jacoco-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-testkit-jacoco-plugin)](https://github.com/gmazzo/gradle-testkit-jacoco-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-testkit-jacoco-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.gradle.testkit.jacoco)](https://plugins.gradle.org/plugin/io.github.gmazzo.gradle.testkit.jacoco)
  [![Build Status](https://github.com/gmazzo/gradle-testkit-jacoco-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-testkit-jacoco-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-testkit-jacoco-plugin/branch/main/graph/badge.svg?token=D5cDiPWvcS)](https://codecov.io/gh/gmazzo/gradle-testkit-jacoco-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.gradle.testkit.jacoco+-repo:github.com/gmazzo/gradle-testkit-jacoco-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-testkit-jacoco-plugin)](https://github.com/gmazzo/gradle-testkit-jacoco-plugin/graphs/contributors)

  ```kotlin
  plugins {
    `java-gradle-plugin`
    id("io.github.gmazzo.gradle.testkit.jacoco") version "<latest>" 
  }
  ```
  
- [`gradle-multiapi-dev-plugin`](https://github.com/gmazzo/gradle-multiapi-dev-plugin)

  A Gradle plugin allows targeting multiple `gradleApi()`s versions.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-multiapi-dev-plugin)](https://github.com/gmazzo/gradle-multiapi-dev-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-multiapi-dev-plugin)](https://github.com/gmazzo/gradle-multiapi-dev-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-multiapi-dev-plugin)](https://github.com/gmazzo/gradle-multiapi-dev-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-multiapi-dev-plugin)](https://github.com/gmazzo/gradle-multiapi-dev-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-multiapi-dev-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.gradle.multiapi)](https://plugins.gradle.org/plugin/io.github.gmazzo.gradle.multiapi)
  [![Build Status](https://github.com/gmazzo/gradle-multiapi-dev-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-multiapi-dev-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-multiapi-dev-plugin/branch/main/graph/badge.svg?token=D5cDiPWvcS)](https://codecov.io/gh/gmazzo/gradle-multiapi-dev-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.gradle.multiapi+-repo:github.com/gmazzo/gradle-multiapi-dev-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-multiapi-dev-plugin)](https://github.com/gmazzo/gradle-multiapi-dev-plugin/graphs/contributors)

  ```kotlin
  plugins {
    `java-gradle-plugin`
    id("io.github.gmazzo.gradle.multiapi") version "<latest>" 
  }

  gradlePlugin {
    apiTargets("7.0", "8.1", "8.13")
  }
  ```
  ![Project Structure](https://github.com/gmazzo/gradle-multiapi-dev-plugin/raw/main/README-structure.png)
    
- [`gradle-aar2jar-plugin`](https://github.com/gmazzo/gradle-aar2jar-plugin)

  A Gradle plugin to allow consuming Android's AAR dependencies as JAR dependencies for JVM projects.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-aar2jar-plugin)](https://github.com/gmazzo/gradle-aar2jar-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-aar2jar-plugin)](https://github.com/gmazzo/gradle-aar2jar-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-aar2jar-plugin)](https://github.com/gmazzo/gradle-aar2jar-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-aar2jar-plugin)](https://github.com/gmazzo/gradle-aar2jar-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-aar2jar-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.aar2jar)](https://plugins.gradle.org/plugin/io.github.gmazzo.aar2jar)
  [![Build Status](https://github.com/gmazzo/gradle-aar2jar-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-aar2jar-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-aar2jar-plugin/branch/main/graph/badge.svg?token=D5cDiPWvcS)](https://codecov.io/gh/gmazzo/gradle-aar2jar-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.aar2jar+-repo:github.com/gmazzo/gradle-aar2jar-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-aar2jar-plugin)](https://github.com/gmazzo/gradle-aar2jar-plugin/graphs/contributors)

  ```kotlin
  plugins {
    java
    id("io.github.gmazzo.aar2jar") version "<latest>" 
  }

  dependencies {
    implementation("androidx.fragment:fragment:1.8.5")
  }
  ```

- [`gradle-codeowners-plugin`](https://github.com/gmazzo/gradle-codeowners-plugin)

  A set of Gradle plugins to propagate CODEOWNERS of classes to runtime for JVM and Kotlin Multiplatform.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-codeowners-plugin)](https://github.com/gmazzo/gradle-codeowners-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-codeowners-plugin)](https://github.com/gmazzo/gradle-codeowners-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-codeowners-plugin)](https://github.com/gmazzo/gradle-codeowners-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-codeowners-plugin)](https://github.com/gmazzo/gradle-codeowners-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-codeowners-plugin)
  [![Maven Central](https://img.shields.io/maven-central/v/io.github.gmazzo.codeowners/matcher)](https://central.sonatype.com/artifact/io.github.gmazzo.codeowners/matcher)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.codeowners)](https://plugins.gradle.org/plugin/io.github.gmazzo.codeowners)
  [![Build Status](https://github.com/gmazzo/gradle-codeowners-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-codeowners-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-codeowners-plugin/branch/main/graph/badge.svg?token=ExYkP1Q9oE)](https://codecov.io/gh/gmazzo/gradle-codeowners-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.codeowners+-repo:github.com/gmazzo/gradle-codeowners-plugin)  
   
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-codeowners-plugin)](https://github.com/gmazzo/gradle-codeowners-plugin/graphs/contributors)

  ```kotlin
  val ownersOfFoo = codeOwnersOf<Foo>()
  ```

- [`gradle-android-manifest-lock-plugin`](https://github.com/gmazzo/gradle-android-manifest-lock-plugin)

  A Gradle plugin for providing .lock file support for AndroidManifest. Useful to control what's introduced by 3rd party dependencies into your Manifest.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-android-manifest-lock-plugin)](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-android-manifest-lock-plugin)](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-android-manifest-lock-plugin)](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-android-manifest-lock-plugin)](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-android-manifest-lock-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.android.manifest.lock)](https://plugins.gradle.org/plugin/io.github.gmazzo.android.manifest.lock)
  [![Build Status](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-android-manifest-lock-plugin/branch/main/graph/badge.svg?token=D5cDiPWvcS)](https://codecov.io/gh/gmazzo/gradle-android-manifest-lock-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.android.manifest.lock+-repo:github.com/gmazzo/gradle-android-manifest-lock-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-android-manifest-lock-plugin)](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/graphs/contributors)

  ```yaml
  main:
    namespace: io.github.gmazzo.android.manifest.lock.demo
    minSDK: 24
    targetSDK: 34
    permissions:
      - android.permission.ACCESS_NETWORK_STATE
      - android.permission.FOREGROUND_SERVICE
  ```

- [`gradle-docker-compose-plugin`](https://github.com/gmazzo/gradle-docker-compose-plugin)

  Spawns Docker Compose environments for Test tasks as a Gradle's `Shared Build Service`.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-docker-compose-plugin)](https://github.com/gmazzo/gradle-docker-compose-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-docker-compose-plugin)](https://github.com/gmazzo/gradle-docker-compose-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-docker-compose-plugin)](https://github.com/gmazzo/gradle-docker-compose-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-docker-compose-plugin)](https://github.com/gmazzo/gradle-docker-compose-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-docker-compose-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.docker.compose)](https://plugins.gradle.org/plugin/io.github.gmazzo.docker.compose)
  [![Build Status](https://github.com/gmazzo/gradle-docker-compose-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-docker-compose-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-docker-compose-plugin/branch/main/graph/badge.svg?token=ExYkP1Q9oE)](https://codecov.io/gh/gmazzo/gradle-docker-compose-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.docker.compose+-repo:github.com/gmazzo/gradle-docker-compose-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-docker-compose-plugin)](https://github.com/gmazzo/gradle-docker-compose-plugin/graphs/contributors)

  ```kotlin
  @Value("\${container.main-app.host}:\${container.main-app.tcp80}")
  private lateinit var appEndpoint: String
  ```

- [`gradle-embedded-dependencies-plugin`](https://github.com/gmazzo/gradle-embedded-dependencies-plugin)

  A Gradle plugin to embed dependencies (A.K.A. `fat` or `uber` jar) in the produced `jar`.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-embedded-dependencies-plugin)](https://github.com/gmazzo/gradle-embedded-dependencies-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-embedded-dependencies-plugin)](https://github.com/gmazzo/gradle-embedded-dependencies-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-embedded-dependencies-plugin)](https://github.com/gmazzo/gradle-embedded-dependencies-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-embedded-dependencies-plugin)](https://github.com/gmazzo/gradle-embedded-dependencies-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-embedded-dependencies-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.dependencies.embedded)](https://plugins.gradle.org/plugin/io.github.gmazzo.dependencies.embedded)
  [![Build Status](https://github.com/gmazzo/gradle-embedded-dependencies-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-embedded-dependencies-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-embedded-dependencies-plugin/branch/main/graph/badge.svg?token=D5cDiPWvcS)](https://codecov.io/gh/gmazzo/gradle-embedded-dependencies-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.dependencies.embedded+-repo:github.com/gmazzo/gradle-embedded-dependencies-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-embedded-dependencies-plugin)](https://github.com/gmazzo/gradle-embedded-dependencies-plugin/graphs/contributors)

  ```kotlin
  plugins {
      java
      id("io.github.gmazzo.dependencies.embedded") version "<latest>" 
  }
  
  dependencies {
      embedded("org.apache.commons:commons-lang3:3.14.0")
  }
  ```

- [`gradle-import-classes-plugin`](https://github.com/gmazzo/gradle-import-classes-plugin)

  A Gradle plugin to import and repackage dependencies [`Proguard`](https://www.guardsquare.com/manual/home) tool.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-import-classes-plugin)](https://github.com/gmazzo/gradle-import-classes-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-import-classes-plugin)](https://github.com/gmazzo/gradle-import-classes-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-import-classes-plugin)](https://github.com/gmazzo/gradle-import-classes-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-import-classes-plugin)](https://github.com/gmazzo/gradle-import-classes-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-import-classes-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.importclasses)](https://plugins.gradle.org/plugin/io.github.gmazzo.importclasses)
  [![Build Status](https://github.com/gmazzo/gradle-import-classes-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-import-classes-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-import-classes-plugin/branch/main/graph/badge.svg?token=D5cDiPWvcS)](https://codecov.io/gh/gmazzo/gradle-import-classes-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.importclasses+-repo:github.com/gmazzo/gradle-import-classes-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-import-classes-plugin)](https://github.com/gmazzo/gradle-import-classes-plugin/graphs/contributors)

  ```kotlin
  // build.gradle.kts
  importClasses {
    repackageTo = "org.test.imported"
    keep("org.apache.commons.lang3.StringUtils")
  }
  
  dependencies {
    importClasses("org.apache.commons:commons-lang3:3.14.0")
  }
  ```
  ```java
  // Foo.java
  package org.test;

  import org.test.imported.StringUtils;

  public class Foo {

    public String swapCase(String string) {
        return StringUtils.swapCase(string);
    }

  }
  ```

- [`gradle-module-kind-plugin`](https://github.com/gmazzo/gradle-module-kind-plugin)

  A Gradle plugin to constrain a multi-module build dependency graph.

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-module-kind-plugin)](https://github.com/gmazzo/gradle-module-kind-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-module-kind-plugin)](https://github.com/gmazzo/gradle-module-kind-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-module-kind-plugin)](https://github.com/gmazzo/gradle-module-kind-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-module-kind-plugin)](https://github.com/gmazzo/gradle-module-kind-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-module-kind-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.modulekind)](https://plugins.gradle.org/plugin/io.github.gmazzo.modulekind)
  [![Build Status](https://github.com/gmazzo/gradle-module-kind-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-module-kind-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-module-kind-plugin/branch/main/graph/badge.svg?token=D5cDiPWvcS)](https://codecov.io/gh/gmazzo/gradle-module-kind-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.modulekind+-repo:github.com/gmazzo/gradle-module-kind-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-module-kind-plugin)](https://github.com/gmazzo/gradle-module-kind-plugin/graphs/contributors)

  ```kotlin
  moduleKindConstraints {
      "implementation" compatibleWith "api"
      "monolith" compatibleWith "implementation"
      "monolith" compatibleWith "api" // redundant, since compatibilities are transitive
  }
  ```
  | `moduleKind`   | api | implementation | monolith |
  | -------------- | --- | -------------- | -------- |
  | api            | ❌   | ❌              | ❌        |
  | implementation | ✅   | ❌              | ❌        |
  | monolith       | ✅   | ✅              | ✅        |

  ![README-failure.png](https://github.com/gmazzo/gradle-module-kind-plugin/raw/main/README-failure.png)

- [`gradle-report-publications-plugin`](https://github.com/gmazzo/gradle-report-publications-plugin)

  A Gradle plugin that decorates the build logs with maven coordinates of artifacts published with `publish` or `publishToMavenLocal`

  [![Stars](https://img.shields.io/github/stars/gmazzo/gradle-report-publications-plugin)](https://github.com/gmazzo/gradle-report-publications-plugin/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/gradle-report-publications-plugin)](https://github.com/gmazzo/gradle-report-publications-plugin/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/gradle-report-publications-plugin)](https://github.com/gmazzo/gradle-report-publications-plugin/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/gradle-report-publications-plugin)](https://github.com/gmazzo/gradle-report-publications-plugin/pulls)
  ![GitHub](https://img.shields.io/github/license/gmazzo/gradle-report-publications-plugin)
  [![Gradle Plugin Portal](https://img.shields.io/gradle-plugin-portal/v/io.github.gmazzo.publications.report)](https://plugins.gradle.org/plugin/io.github.gmazzo.publications.report)
  [![Build Status](https://github.com/gmazzo/gradle-report-publications-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/gradle-report-publications-plugin/actions/workflows/build.yaml)
  [![Coverage](https://codecov.io/gh/gmazzo/gradle-report-publications-plugin/branch/main/graph/badge.svg?token=D5cDiPWvcS)](https://codecov.io/gh/gmazzo/gradle-report-publications-plugin)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:io.github.gmazzo.publications.report+-repo:github.com/gmazzo/gradle-report-publications-plugin)
  
  [![Contributors](https://contrib.rocks/image?repo=gmazzo/gradle-report-publications-plugin)](https://github.com/gmazzo/gradle-report-publications-plugin/graphs/contributors)

  ![publications](https://github.com/gmazzo/gradle-report-publications-plugin/raw/main/README-example-output.png)

### Docker images
- [`kotlin-container`](https://github.com/gmazzo/kotlin-container)

  An unofficial Docker image for running Kotlin scripts.
  
  [![Stars](https://img.shields.io/github/stars/gmazzo/kotlin-container)](https://github.com/gmazzo/kotlin-container/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/kotlin-container)](https://github.com/gmazzo/kotlin-container/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/kotlin-container)](https://github.com/gmazzo/kotlin-container/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/kotlin-container)](https://github.com/gmazzo/kotlin-container/pulls)
  [![Latest](https://img.shields.io/docker/image-size/gmazzo/kotlin)](https://hub.docker.com/repository/docker/gmazzo/kotlin/general)
  [![Build Status](https://github.com/gmazzo/kotlin-container/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/kotlin-container/actions/workflows/build.yaml)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:gmazzo/kotlin-container%40+-repo:github.com/gmazzo/kotlin-container)

  [![Contributors](https://contrib.rocks/image?repo=gmazzo/kotlin-container)](https://github.com/gmazzo/kotlin-container/graphs/contributors)

  ```bash
  docker run -v ./scripts:/scripts gmazzo/kotlin /scripts/hello.kts
  ```

### GitHub Actions
- [`publish-report-annotations`](https://github.com/gmazzo/publish-report-annotations)

  Reports `JUnit`, `Android Lint`, `Detekt` and any other `CheckStyle` compatible `XML` reports as GitHub Actions annotations. Mostly targeting `Gradle` builds

  [![Stars](https://img.shields.io/github/stars/gmazzo/publish-report-annotations)](https://github.com/gmazzo/publish-report-annotations/stargazers)
  [![Forks](https://img.shields.io/github/forks/gmazzo/publish-report-annotations)](https://github.com/gmazzo/publish-report-annotations/forks)
  [![Issues](https://img.shields.io/github/issues/gmazzo/publish-report-annotations)](https://github.com/gmazzo/publish-report-annotations/issues)
  [![PRs](https://img.shields.io/github/issues-pr/gmazzo/publish-report-annotations)](https://github.com/gmazzo/publish-report-annotations/pulls)
  [![Latest](https://img.shields.io/github/v/release/gmazzo/publish-report-annotations)](https://github.com/gmazzo/publish-report-annotations/releases/latest)
  [![Build Status](https://github.com/gmazzo/publish-report-annotations/actions/workflows/build.yaml/badge.svg)](https://github.com/gmazzo/publish-report-annotations/actions/workflows/build.yaml)
  [![codecov](https://codecov.io/gh/gmazzo/publish-report-annotations/branch/main/graph/badge.svg)](https://codecov.io/gh/gmazzo/publish-report-annotations)
  [![Users](https://img.shields.io/badge/users_by-Sourcegraph-purple)](https://sourcegraph.com/search?q=content:gmazzo/publish-report-annotations%40+-repo:github.com/gmazzo/publish-report-annotations)

  [![Contributors](https://contrib.rocks/image?repo=gmazzo/publish-report-annotations)](https://github.com/gmazzo/publish-report-annotations/graphs/contributors)

  ```yaml
  steps:
    - name: Run Gradle build
      run: ./gradlew build # this is an example
    - name: Report build results
      uses: gmazzo/publish-report-annotations@v1 # target latest major
      if: ${{ !cancelled() }}
  ```
  ![PR status check](https://github.com/gmazzo/publish-report-annotations/assets/513566/434289a0-6d4d-4226-ad4c-49554080df80)

  | Test Suites                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | ✅ 93 passed | 🟡 1 skipped | ❌ 4 failed | ⌛ took |
  |:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------|--------------|------------|--------|
  | <details><summary>✅ org.test.sample.AnotherTestSuite</summary><ul><li>✅ aTest[maxDuration=100] (⌛ 0.054)</li><li>✅ aTest[maxDuration=200] (⌛ 0.107)</li><li>✅ aTest[maxDuration=300] (⌛ 0.238)</li><li>✅ aTest[maxDuration=400] (⌛ 0.103)</li></ul></details>                                                                                                                                                                                                                                                                                                              | 4           | 0            | 0          | 0.506  |
  | <details><summary>❌ org.test.sample.FlakyFailingTestSuite</summary><ul><li>❌ failingTest() (⌛ 0.011)</li></ul></details>                                                                                                                                                                                                                                                                                                                                                                                                                                                   | 0           | 0            | 1          | 2.07   |
  | <details><summary>❎❗org.test.sample.FlakyTestSuite [^flakyDisclaimer]</summary><ul><li>❎❗[^flakyDisclaimer]flakyTest() (⌛ 0.005)</li></ul></details>                                                                                                                                                                                                                                                                                                                                                                                                                       | 1           | 0            | 0          | 1.295  |
  | <details><summary>❌ org.test.sample.SampleTestSuite</summary><ul><li>🟡 a test skipped() (⌛ 0)</li><li>❌ a test that fails() (⌛ 0.002)</li><li>✅ a test that passes() (⌛ 0.001)</li><li>❌ a test that throws an exception() (⌛ 0.001)</li></ul></details>                                                                                                                                                                                                                                                                                                                  | 1           | 1            | 2          | 0.004  |
  
  [^flakyDisclaimer]: ❎❗flaky test (some executions have passed, others have failed)

  ![junit](https://github.com/gmazzo/publish-report-annotations/assets/513566/57ba4328-0318-48b5-9d91-22113c4387bb)
  ![lint](https://github.com/gmazzo/gmazzo/assets/513566/23ddef4c-186c-444f-8355-c599b3645630)
