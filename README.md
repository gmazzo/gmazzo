# Guillermo Mazzola [![LinkedIn Profile](https://img.shields.io/badge/-gmazzo-0d65c2?logo=linkedin)](https://www.linkedin.com/in/gmazzo/)
[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=gmazzo&theme=onedark&count_private=true&hide_title=true&show_icons=true)](https://github.com/anuraghazra/github-readme-stats)

## Portfolio of open source projects

### JVM libraries
- [`okhttp-client-mock`](https://github.com/gmazzo/okhttp-client-mock)<br/>
  A simple `OKHttp` client mock, using a programmable request interceptor
  ```kotlin
  val interceptor = MockInterceptor()
  
  interceptor.rule(url eq "https://testserver/api/json") {
    respond("{succeed:true}", MEDIATYPE_JSON)
  }
  ```
  [![stars](https://img.shields.io/github/stars/gmazzo/okhttp-client-mock)](https://github.com/gmazzo/okhttp-client-mock/stargazers)
  [![stars](https://img.shields.io/github/issues/gmazzo/okhttp-client-mock)](https://github.com/gmazzo/okhttp-client-mock/issues)
  [![stars](https://img.shields.io/github/issues-pr/gmazzo/okhttp-client-mock)](https://github.com/gmazzo/okhttp-client-mock/pulls)

### Gradle plugins
- [`gradle-buildconfig-plugin`](https://github.com/gmazzo/gradle-buildconfig-plugin)<br/>
  A plugin for generating BuildConstants for any kind of Gradle projects: Java, Kotlin, Groovy, etc. Designed for KTS scripts.<br/>
  ```kotlin
  buildConfig {
    buildConfigField("APP_NAME", project.name)
    buildConfigField("APP_VERSION", provider { "${project.version}" })
  ```
  [![stars](https://img.shields.io/github/stars/gmazzo/gradle-buildconfig-plugin)](https://github.com/gmazzo/gradle-buildconfig-plugin/stargazers)
  [![stars](https://img.shields.io/github/issues/gmazzo/gradle-buildconfig-plugin)](https://github.com/gmazzo/gradle-buildconfig-plugin/issues)
  [![stars](https://img.shields.io/github/issues-pr/gmazzo/gradle-buildconfig-plugin)](https://github.com/gmazzo/gradle-buildconfig-plugin/pulls)
  
- [`gradle-android-test-aggregation-plugin`](https://github.com/gmazzo/gradle-android-test-aggregation-plugin)<br/>
  A couple Gradle plugins to make Android modules to work with [JaCoCo Report Aggregation Plugin](https://docs.gradle.org/current/userguide/jacoco_report_aggregation_plugin.html) and [Test Report Aggregation Plugin](https://docs.gradle.org/current/userguide/test_report_aggregation_plugin.html)<br/>
  ![aggregated-jacoco-report](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/raw/main/README-aggregated-jacoco-report.png)<br/>
  [![stars](https://img.shields.io/github/stars/gmazzo/gradle-android-test-aggregation-plugin)](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/stargazers)
  [![stars](https://img.shields.io/github/issues/gmazzo/gradle-android-test-aggregation-plugin)](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/issues)
  [![stars](https://img.shields.io/github/issues-pr/gmazzo/gradle-android-test-aggregation-plugin)](https://github.com/gmazzo/gradle-android-test-aggregation-plugin/pulls)
  
- [`gradle-codeowners-plugin`](https://github.com/gmazzo/gradle-codeowners-plugin)<br/>
  A set of Gradle plugins to propagate CODEOWNERS of classes to runtime for JVM and Kotlin Multiplatform.
  ```kotlin
  val ownersOfFoo = codeOwnersOf<Foo>()
  ```
  [![stars](https://img.shields.io/github/stars/gmazzo/gradle-codeowners-plugin)](https://github.com/gmazzo/gradle-codeowners-plugin/stargazers)
  [![stars](https://img.shields.io/github/issues/gmazzo/gradle-codeowners-plugin)](https://github.com/gmazzo/gradle-codeowners-plugin/issues)
  [![stars](https://img.shields.io/github/issues-pr/gmazzo/gradle-codeowners-plugin)](https://github.com/gmazzo/gradle-codeowners-plugin/pulls)
  
- [`gradle-android-manifest-lock-plugin`](https://github.com/gmazzo/gradle-android-manifest-lock-plugin)<br/>
  A Gradle plugin for providing .lock file support for AndroidManifest. Useful to control what's introduced by 3rd party dependencies into your Manifest.
  ```yaml
  main:
    namespace: io.github.gmazzo.android.manifest.lock.demo
    minSDK: 24
    targetSDK: 34
    permissions:
      - android.permission.ACCESS_NETWORK_STATE
      - android.permission.FOREGROUND_SERVICE
  ```
  [![stars](https://img.shields.io/github/stars/gmazzo/gradle-android-manifest-lock-plugin)](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/stargazers)
  [![stars](https://img.shields.io/github/issues/gmazzo/gradle-android-manifest-lock-plugin)](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/issues)
  [![stars](https://img.shields.io/github/issues-pr/gmazzo/gradle-android-manifest-lock-plugin)](https://github.com/gmazzo/gradle-android-manifest-lock-plugin/pulls)
  
- [`gradle-docker-compose-plugin`](https://github.com/gmazzo/gradle-docker-compose-plugin)<br/>
  Spawns Docker Compose environments for Test tasks as a Gradle's `Shared Build Service`.
  ```kotlin
  @Value("\${container.main-app.host}:\${container.main-app.tcp80}")
  private lateinit var appEndpoint: String
  ```
  [![stars](https://img.shields.io/github/stars/gmazzo/gradle-docker-compose-plugin)](https://github.com/gmazzo/gradle-docker-compose-plugin/stargazers)
  [![stars](https://img.shields.io/github/issues/gmazzo/gradle-docker-compose-plugin)](https://github.com/gmazzo/gradle-docker-compose-plugin/issues)
  [![stars](https://img.shields.io/github/issues-pr/gmazzo/gradle-docker-compose-plugin)](https://github.com/gmazzo/gradle-docker-compose-plugin/pulls)
  
- [`gradle-report-publications-plugin`](https://github.com/gmazzo/gradle-report-publications-plugin)<br/>
  A Gradle plugin that decorates the build logs with maven coordinates of artifacts published with `publish` or `publishToMavenLocal`<br/>
  ![publications](https://github.com/gmazzo/gradle-report-publications-plugin/raw/main/README-example-output.png)<br/>
  [![stars](https://img.shields.io/github/stars/gmazzo/gradle-report-publications-plugin)](https://github.com/gmazzo/gradle-report-publications-plugin/stargazers)
  [![stars](https://img.shields.io/github/issues/gmazzo/gradle-report-publications-plugin)](https://github.com/gmazzo/gradle-report-publications-plugin/issues)
  [![stars](https://img.shields.io/github/issues-pr/gmazzo/gradle-report-publications-plugin)](https://github.com/gmazzo/gradle-report-publications-plugin/pulls)
  
