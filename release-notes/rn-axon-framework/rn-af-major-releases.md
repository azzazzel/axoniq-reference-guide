# Major Releases

All the enhancements and features which have been introduced to our major releases of the Axon Framework are noted here.

## Release 4.6

Axon Framework 4.6.0 has undergone a great deal of changes.
Some noteworthy additions are the [Dead-Letter Queue](https://github.com/AxonFramework/AxonFramework/pull/2258), [integrated Tracing with Open Telemetry](https://github.com/AxonFramework/AxonFramework/pull/2294) and [Jakarta support](https://github.com/AxonFramework/AxonFramework/pull/2301).
For an exhaustive list of the features, enhancements, and bug fixes with introduced, see below.
For a list that also contains the dependency upgrades we refer to [this](https://github.com/AxonFramework/AxonFramework/releases/tag/axon-4.6.0) page.

### _Features_

- Added Slack release announcement [#2348](https://github.com/AxonFramework/AxonFramework/pull/2348)
- [#2307] Carry the context during reset to the `ReplayToken` [#2312](https://github.com/AxonFramework/AxonFramework/pull/2312)
- Propagate ResetContext in ReplayToken [#2307](https://github.com/AxonFramework/AxonFramework/issues/2307)
- [#2198] Add support for Jakarta [#2301](https://github.com/AxonFramework/AxonFramework/pull/2301)
- Native Tracing for Axon Framework with OpenTelemetry as default [#2294](https://github.com/AxonFramework/AxonFramework/pull/2294)
- [#2021] Dead Letter Queue for Event Processing Groups [#2258](https://github.com/AxonFramework/AxonFramework/pull/2258)
- JPA dead letter queue implementation [#2239](https://github.com/AxonFramework/AxonFramework/pull/2239)
- Construct means to switch between classes using `javax` and `jakarta` [#2198](https://github.com/AxonFramework/AxonFramework/issues/2198)
- Create add-dependabot-pr-to-project.yml [#2183](https://github.com/AxonFramework/AxonFramework/pull/2183)
- Create add-issues-to-project.yml [#2182](https://github.com/AxonFramework/AxonFramework/pull/2182)
- Multiteant support [#2156](https://github.com/AxonFramework/AxonFramework/pull/2156)
- Spring event for indication that Axon has started [#2146](https://github.com/AxonFramework/AxonFramework/pull/2146)
- Application events when handlers are registered [#2144](https://github.com/AxonFramework/AxonFramework/pull/2144)
- [#1125] Introduce `SagaLifecycle.associationValues()` [#2141](https://github.com/AxonFramework/AxonFramework/pull/2141)
- [#1964] Include `AxonServerHealthIndicator` [#2130](https://github.com/AxonFramework/AxonFramework/pull/2130)
- `AggregateTestFixture` improvement - Validate Exception Details [#2125](https://github.com/AxonFramework/AxonFramework/pull/2125)
- `AggregateTestFixture` improvement - Validate Exception Details [#2110](https://github.com/AxonFramework/AxonFramework/issues/2110)
- Feature/1466 Additional deadline validation methods [#2071](https://github.com/AxonFramework/AxonFramework/pull/2071)
- Multi-tenant support [#2045](https://github.com/AxonFramework/AxonFramework/pull/2045)
- Dead-Letter Queue for Event Processors [#2021](https://github.com/AxonFramework/AxonFramework/issues/2021)
- Added AxonServerEEContainer and AxonServerSEContainer as an easier way for people to write tests [#2020](https://github.com/AxonFramework/AxonFramework/pull/2020)
- Streaming query [#2001](https://github.com/AxonFramework/AxonFramework/pull/2001)
- [#1967] Fetch available segements only from the TokenStore [#1997](https://github.com/AxonFramework/AxonFramework/pull/1997)
- [#1645] Introduce ObjectNode-to/from-JsonNode `ContentTypeConverter` for the `JacksonSerializer` [#1995](https://github.com/AxonFramework/AxonFramework/pull/1995)
- [#1490] Simplify LockFactory configuration for Aggregates [#1992](https://github.com/AxonFramework/AxonFramework/pull/1992)
- [#1986 Introduce `EventProcessingConfigurer#defaultTransactionManager` method [#1989](https://github.com/AxonFramework/AxonFramework/pull/1989)
- Register default Transaction Manager through Event Processing Configurer [#1986](https://github.com/AxonFramework/AxonFramework/issues/1986)
- Add method returning the available segments of a TokenStore [#1967](https://github.com/AxonFramework/AxonFramework/issues/1967)
- Add an actuator health indicator to check the connection between the application and Axon Server [#1964](https://github.com/AxonFramework/AxonFramework/issues/1964)
- Added the MetaDataSequencingPolicy [#1930](https://github.com/AxonFramework/AxonFramework/pull/1930)
- Provide a SequencingPolicy based on a MetaData field [#1929](https://github.com/AxonFramework/AxonFramework/issues/1929)
- Added an option to create a fixture for a state stored aggregate [#1772](https://github.com/AxonFramework/AxonFramework/pull/1772)
- JsonNode-to-ObjectNode ContentTypeConverter [#1645](https://github.com/AxonFramework/AxonFramework/issues/1645)
- Simplify LockFactory configuration per aggregate [#1490](https://github.com/AxonFramework/AxonFramework/issues/1490)
- Additional Deadline Validation methods. [#1466](https://github.com/AxonFramework/AxonFramework/issues/1466)
- Allow TrackingEventProcessor start to be deferred [#1184](https://github.com/AxonFramework/AxonFramework/pull/1184)
- Accessing Saga Association Values [#1125](https://github.com/AxonFramework/AxonFramework/issues/1125)
- Signal when all Handlers have been registered in Spring environment [#880](https://github.com/AxonFramework/AxonFramework/issues/880)

### _Enhancements_

- Improve deadline span name. [#2360](https://github.com/AxonFramework/AxonFramework/pull/2360)
- Make Given-phase Error Handling configurable for Saga Test Fixtures [#2356](https://github.com/AxonFramework/AxonFramework/pull/2356)
- Improve SpanFactory autoconfiguration mechanism. [#2354](https://github.com/AxonFramework/AxonFramework/pull/2354)
- Introduce LoggingSpanFactory and MultiSpanFactory [#2353](https://github.com/AxonFramework/AxonFramework/pull/2353)
- Check if a certain handler contains certain methods before registering it. [#2346](https://github.com/AxonFramework/AxonFramework/pull/2346)
- Catch exceptions from correlation data providers. [#2345](https://github.com/AxonFramework/AxonFramework/pull/2345)
- Throw exception on ambiguous dependencies [#2344](https://github.com/AxonFramework/AxonFramework/pull/2344)
- Integration Test for Command and Query Priority Calculations [#2342](https://github.com/AxonFramework/AxonFramework/pull/2342)
- Include message identifier in error message if de-serialization fails [#2330](https://github.com/AxonFramework/AxonFramework/pull/2330)
- Add CorrelationDataProvider error handling on rollback [#2328](https://github.com/AxonFramework/AxonFramework/issues/2328)
- Strip test prefix once required in JUnit 3 from test method names [#2321](https://github.com/AxonFramework/AxonFramework/pull/2321)
- Apache Maven Wrapper 3.8.6 [#2320](https://github.com/AxonFramework/AxonFramework/pull/2320)
- Allow ReplayToken creation to be customizable when resetting a projection [#2308](https://github.com/AxonFramework/AxonFramework/pull/2308)
- Ensure all dispatchable messages are serialiable by Jackson and Xstream. [#2295](https://github.com/AxonFramework/AxonFramework/pull/2295)
- Testclasses for javax jakarta extension [#2280](https://github.com/AxonFramework/AxonFramework/pull/2280)
- Remove redundant method definition [#2270](https://github.com/AxonFramework/AxonFramework/pull/2270)
- Integration Test for Command and Query Priority Calculations [#2266](https://github.com/AxonFramework/AxonFramework/pull/2266)
- Update the `PrioritizedRunnable` to a `PriorityTask` [#2265](https://github.com/AxonFramework/AxonFramework/pull/2265)
- Automatically add Release Notes on milestone closure to Discuss post [#2264](https://github.com/AxonFramework/AxonFramework/pull/2264)
- Create a protected method to fetch tracking events on JpaEventStorageEngine [#2262](https://github.com/AxonFramework/AxonFramework/pull/2262)
- Create a protected method to fetch tracking events on JpaEventStorageEngine. [#2259](https://github.com/AxonFramework/AxonFramework/pull/2259)
- Allow subtype definition on the `Repository` builders for Polymorphic Aggregates [#2250](https://github.com/AxonFramework/AxonFramework/pull/2250)
- Add test for ConsistentHash.equals [#2244](https://github.com/AxonFramework/AxonFramework/pull/2244)
- Use getHost instead of getContainerIpAddress [#2222](https://github.com/AxonFramework/AxonFramework/pull/2222)
- Default snapshotfilter with revision null [#2213](https://github.com/AxonFramework/AxonFramework/pull/2213)
- Default snapshot filter with revision null [#2212](https://github.com/AxonFramework/AxonFramework/pull/2212)
- Creation policy factory for Aggregates [#2209](https://github.com/AxonFramework/AxonFramework/pull/2209)
- Removed deprecated code by updating the default serializer initialization [#2206](https://github.com/AxonFramework/AxonFramework/pull/2206)
- Flux response type rank matching [#2197](https://github.com/AxonFramework/AxonFramework/pull/2197)
- Introduce conditional variants for `ApplyMore` [#2174](https://github.com/AxonFramework/AxonFramework/pull/2174)
- Conditional variant for the ApplyMore methods [#2173](https://github.com/AxonFramework/AxonFramework/issues/2173)
- Take into account the result of the `equals` method before attempting… [#2171](https://github.com/AxonFramework/AxonFramework/pull/2171)
- Improve javadoc of the ReplayStatus enum to reflect changes to the StreamingEventProcessors [#2170](https://github.com/AxonFramework/AxonFramework/pull/2170)
- MultipleInstancesResponseType should match (lower) on single item [#2148](https://github.com/AxonFramework/AxonFramework/pull/2148)
- Add duplicate resolution on query handler registration, defaulting to… [#2140](https://github.com/AxonFramework/AxonFramework/pull/2140)
- Add method on DefaultCommandGateway to be able to customize callbacks [#2139](https://github.com/AxonFramework/AxonFramework/pull/2139)
- Default Revision `SnapshotFilter` in absence of annotation [#2136](https://github.com/AxonFramework/AxonFramework/issues/2136)
- Fine tune the `MessageHandlerLookup` for Spring Native support [#2106](https://github.com/AxonFramework/AxonFramework/pull/2106)
- Redesign of Spring Boot Auto Configuration support [#2105](https://github.com/AxonFramework/AxonFramework/pull/2105)
- Feature/1629 saga test fixture [#2101](https://github.com/AxonFramework/AxonFramework/pull/2101)
- [#2093] Validate if target Command Handling Member can resolve target [#2095](https://github.com/AxonFramework/AxonFramework/pull/2095)
- Allow several Aggregate Member collections of the same type [#2093](https://github.com/AxonFramework/AxonFramework/issues/2093)
- Changed logging about "processor falling behind" [#2073](https://github.com/AxonFramework/AxonFramework/pull/2073)
- Make asDomainEventMessage available to subclasses [#2066](https://github.com/AxonFramework/AxonFramework/pull/2066)
- Make `JpaEventStorageEngine#asDomainEventMessage(EventMessage<?>)` protected [#2065](https://github.com/AxonFramework/AxonFramework/issues/2065)
- Separate Integration Tests and Aggregate coverage reports [#2063](https://github.com/AxonFramework/AxonFramework/pull/2063)
- [#1646] Update "No Handler For" exceptional cases [#2062](https://github.com/AxonFramework/AxonFramework/pull/2062)
- [#1711] Simplify attachment of Lifecycle Operations [#2061](https://github.com/AxonFramework/AxonFramework/pull/2061)
- Change how Sonar is invoked for GHA's [#2033](https://github.com/AxonFramework/AxonFramework/pull/2033)
- Introduce LifecycleAware interface for managing component lifecycle [#2028](https://github.com/AxonFramework/AxonFramework/pull/2028)
- Remove MonoWrapper usage. [#2008](https://github.com/AxonFramework/AxonFramework/pull/2008)
- Replaced `method.getParametersTypes().length` by `method.getParameterCount())` [#1987](https://github.com/AxonFramework/AxonFramework/pull/1987)
- Methods for testing deadlines when time passed are consistent in TestExecutor & SagaTestFixture (fixes #1974) [#1975](https://github.com/AxonFramework/AxonFramework/pull/1975)
- Make methods for testing Deadlines consistent for `TestExecutor` and `SagaTestFixture` [#1974](https://github.com/AxonFramework/AxonFramework/issues/1974)
- Added jdk17-ea on our build workflow for early feedback [#1915](https://github.com/AxonFramework/AxonFramework/pull/1915)
- Add configurable options for checking failure transiency [#1910](https://github.com/AxonFramework/AxonFramework/pull/1910)
- Prevent stack trace generation for HandlerExecutionException [#1905](https://github.com/AxonFramework/AxonFramework/pull/1905)
- Allow creation of HandlerExecutionExceptions without stacktrace [#1901](https://github.com/AxonFramework/AxonFramework/issues/1901)
- [#1898] Empty associationProperty leads to IndexOutOfBoundsException [#1899](https://github.com/AxonFramework/AxonFramework/pull/1899)
- Empty associationProperty leads to IndexOutOfBoundsException [#1898](https://github.com/AxonFramework/AxonFramework/issues/1898)
- Provide means of configuring a `CommandCallback` [#1889](https://github.com/AxonFramework/AxonFramework/issues/1889)
- Splitted builds into pr and not pr, added ghactions to dependabot and other minors [#1830](https://github.com/AxonFramework/AxonFramework/pull/1830)
- Fine tune triggered Deadline validation for Test Fixtures  [#1797](https://github.com/AxonFramework/AxonFramework/pull/1797)
- Simplified DeadlineManager configuration [#1796](https://github.com/AxonFramework/AxonFramework/pull/1796)
- Expand RetryScheduler to support more granular decision when to retry [#1723](https://github.com/AxonFramework/AxonFramework/issues/1723)
- Simplify attachment of Lifecycle Operations [#1711](https://github.com/AxonFramework/AxonFramework/issues/1711)
- Improved termination heuristic when response is < batchsize/2 and the… [#1691](https://github.com/AxonFramework/AxonFramework/pull/1691)
- Exception in startHandlers is "swallowed" by exception in shutdownHandlers [#1669](https://github.com/AxonFramework/AxonFramework/issues/1669)
- Fine tune "No Handler For..." Exception [#1646](https://github.com/AxonFramework/AxonFramework/issues/1646)
- SagaTestFixture should support expectSuccessfulHandlerExecution() [#1629](https://github.com/AxonFramework/AxonFramework/issues/1629)
- Large number of rolled back transactions on JPA/JDBC TokenStore [#1475](https://github.com/AxonFramework/AxonFramework/issues/1475)
- Reduce Reflection usage [#1427](https://github.com/AxonFramework/AxonFramework/issues/1427)
- Add annotation NonNull/Nullable for better usage in kotlin (also java) [#1280](https://github.com/AxonFramework/AxonFramework/issues/1280)
- Spurious warnings when a tracking token gap appears then is filled [#1193](https://github.com/AxonFramework/AxonFramework/issues/1193)
- Query handlers of the same name and response type within one class [#719](https://github.com/AxonFramework/AxonFramework/issues/719)
- MultipleInstancesResponseType should recognize handler with single result [#602](https://github.com/AxonFramework/AxonFramework/issues/602)

### _Bug Fixes_

- Rename SpanFactory.registerTagProvider to registerSpanAttributeProvider [#2347](https://github.com/AxonFramework/AxonFramework/pull/2347)
- [#2341] Adjust type checking in `SimpleQueryUpdateEmitter` to accompany type erasure [#2343](https://github.com/AxonFramework/AxonFramework/pull/2343)
- UpdateEmitter drops MultipleInstancesResponseType updates due to type checking. [#2341](https://github.com/AxonFramework/AxonFramework/issues/2341)
- Parameter resolver ordering is wrong for test fixtures [#2340](https://github.com/AxonFramework/AxonFramework/pull/2340)
- Take all types into account when resolving the deadline handler [#2336](https://github.com/AxonFramework/AxonFramework/pull/2336)
- When moving to a polymorphic Aggregate the stored Deadlines are not handled. [#2333](https://github.com/AxonFramework/AxonFramework/issues/2333)
- [#2331] Fix deserialization bug `GrpcBackedSubscriptionQueryMessage` and filter non-handler-matching updates [#2332](https://github.com/AxonFramework/AxonFramework/pull/2332)
- `GrpcBackedSubscriptionQueryMessage` overwrites update type with initial response type [#2331](https://github.com/AxonFramework/AxonFramework/issues/2331)
- [#2317] Using deadlines with DefaultConfigurer leads to NPE [#2319](https://github.com/AxonFramework/AxonFramework/pull/2319)
- Using deadlines with DefaultConfigurer leads to NPE [#2317](https://github.com/AxonFramework/AxonFramework/issues/2317)
- Fix streaming queries not respecting PriorityTask mechanism [#2309](https://github.com/AxonFramework/AxonFramework/pull/2309)
- [#2268] Adjust `ConditionalOnClass` to validate existence of the `AxonServerConnectionManager` in absence of the `axon-server-connector` package. [#2269](https://github.com/AxonFramework/AxonFramework/pull/2269)
- Bug when using Spring actuator starter and excluding axon server [#2268](https://github.com/AxonFramework/AxonFramework/issues/2268)
- Support `Cache` and `LockFactory` configuration on `@Aggregate` stereotype [#2254](https://github.com/AxonFramework/AxonFramework/pull/2254)
- Extracted lambdas to inner static classes [#2240](https://github.com/AxonFramework/AxonFramework/pull/2240)
- Dependency on reactor is needed to be able to start an Axon app using current 4.6.0-SNAPSHOT [#2238](https://github.com/AxonFramework/AxonFramework/issues/2238)
- Fix snapshots not being deployed to nexus [#2237](https://github.com/AxonFramework/AxonFramework/pull/2237)
- fix javadoc: default port is 8124, not 8123 [#2223](https://github.com/AxonFramework/AxonFramework/pull/2223)
- fix typo in local variable name [#2218](https://github.com/AxonFramework/AxonFramework/pull/2218)
- Publisher Response Type [#2215](https://github.com/AxonFramework/AxonFramework/pull/2215)
- EventProcessingModule should lazily initialize processors [#2180](https://github.com/AxonFramework/AxonFramework/pull/2180)
- Fix `StreamingEventProcessor#maxCapacity` for the `TrackingEventProcessor` [#2124](https://github.com/AxonFramework/AxonFramework/pull/2124)
- Restore missing commit 6e531a6cf173243adf9519905f42cbec0a334238 [#2116](https://github.com/AxonFramework/AxonFramework/pull/2116)
- Wire eventSerializer into QuartzEventSchedulerFactoryBean [#2115](https://github.com/AxonFramework/AxonFramework/pull/2115)
- Wire the event `Serializer` into `QuartzEventSchedulerFactoryBean` [#2088](https://github.com/AxonFramework/AxonFramework/issues/2088)
- Fix typo in pom.xml [#2022](https://github.com/AxonFramework/AxonFramework/pull/2022)
- Fix typos [#2016](https://github.com/AxonFramework/AxonFramework/pull/2016)
- Exponential Retry for Tracking event processor not happening for transient exceptions when using postgres JdbcTokenStore [#1920](https://github.com/AxonFramework/AxonFramework/issues/1920)

### _Contributors_

We'd like to thank all the contributors who worked on this release!

- [@mnegacz](https://github.com/mnegacz)
- [@WackyS](https://github.com/WackyS)
- [@YvonneCeelie](https://github.com/YvonneCeelie)
- [@altuntasfatih](https://github.com/altuntasfatih)
- [@saratry](https://github.com/saratry)
- [@barbeque-squared](https://github.com/barbeque-squared)
- [@srmppn](https://github.com/srmppn)
- [@krosenvold](https://github.com/krosenvold)
- [@gklijs](https://github.com/gklijs)
- [@erikhofer](https://github.com/erikhofer)
- [@Dilsh0d](https://github.com/Dilsh0d)
- [@smcvb](https://github.com/smcvb)
- [@sandjelkovic](https://github.com/sandjelkovic)
- [@MGathier](https://github.com/MGathier)
- [@dgomezg](https://github.com/dgomezg)
- [@Arnaud-J](https://github.com/Arnaud-J)
- [@sascha-eisenmann](https://github.com/sascha-eisenmann)
- [@Morlack](https://github.com/Morlack)
- [@andye2004](https://github.com/andye2004)
- [@nils-christian](https://github.com/nils-christian)
- [@lfgcampos](https://github.com/lfgcampos)
- [@heutelbeck](https://github.com/heutelbeck)
- [@mikelhamer](https://github.com/mikelhamer)
- [@m1l4n54v1c](https://github.com/m1l4n54v1c)
- [@Vermorkentech](https://github.com/Vermorkentech)
- [@lacinoire](https://github.com/lacinoire)
- [@jangalinski](https://github.com/jangalinski)
- [@azzazzel](https://github.com/azzazzel)
- [@eddumelendez](https://github.com/eddumelendez)
- [@timtebeek](https://github.com/timtebeek)
- [@sgrimm-sg](https://github.com/sgrimm-sg)
- [@dmurat](https://github.com/dmurat)
- [@abuijze](https://github.com/abuijze)
- [@hatzlj](https://github.com/hatzlj)
- [@schananas](https://github.com/schananas)

## Release 4.5

This release has seen numerous addition towards Axon Framework.
The most interesting adjustments can be seen down below. 
Note that the BOM (as marked in [#1200](https://github.com/AxonFramework/AxonFramework/issues/1200)) is not part of the release notes, as this will use its own separate release cycle.
For those interested, the BOM repository can be found [here](https://github.com/AxonFramework/axon-bom).

For an exhaustive list of all adjustments made for release 4.5 you can check out [this](https://github.com/AxonFramework/AxonFramework/releases/tag/axon-4.5) page.

### _Enhancements_

* A new type of `EventProcessor` has been introduced in pull request [#1712](https://github.com/AxonFramework/AxonFramework/pull/1712), called the `PooledStreamingEventProcessor`.
  This `EventProcessor` allows the same set of operations as the `TrackingEventProcessor`, but uses a different threading approach for handling events and processing operations.
  In all, this solution provides a more straightforward processor implementation and configuration, allowing for enhanced event processing in general.
  For specifics on how to configure it, check out [this](../../axon-framework/events/event-processors/streaming.md#pooled-streaming-event-processor) section.
  
* Sagas support the use of [Deadline Handlers](../../axon-framework/deadlines/deadline-managers.md#handling-a-deadline), but an `@DeadlineHandler` annotated method couldn't automatically close a Saga with the `@EndSaga` annotation.
  This enhancement has been described in [#1469](https://github.com/AxonFramework/AxonFramework/issues/1469) and resolved in pull request [#1656](https://github.com/AxonFramework/AxonFramework/pull/1656).
  As such, as of Axon 4.5, an `@DeadlineHandler` annotated can also be annotated with `@EndSaga`, to automatically close the Saga whenever the given deadline is handled.
  
* Whenever an application uses snapshots, the point arises that old snapshot versions need to be invalidated when loading an Aggregate.
  To that end the [`SnapshotFilter`](../../axon-framework/tuning/event-snapshots.md#filtering-snapshot-events) can be configured.
  As a simplified solution, the `@Revision` annotation can now be placed on the Aggregate class to automatically configure a revision based `SnapshotFilter`.
  Due to this, old snapshots will be filtered out automatically when an Aggregate is reconstructed from the `EventStore`.
  For those interested, the implementation of this feature can be found [here](https://github.com/AxonFramework/AxonFramework/pull/1657).
  
* At the basis of Axon's message handling functionality, is the `MessageHandlingMember`.
  For the time being, the sole implementation of this is the `AnnotatedMessageHandlingMember`, which expect the use of annotations like the `@CommandHandler` and `@EventHandler`, for example.
  As a step towards constructing an annotation-less approach, [#1621](https://github.com/AxonFramework/AxonFramework/pull/1621) was introduced into the framework.
  The first steps taken in this pull request are the deprecation of annotation-specific methods from the `MessageHandlingMember` interface.
  Added to this is a new approach towards defining attributes of a message handling member through `HandlerAttributes`.

### _Bug Fixes_

* The `InMemoryEventStorageEngine` is a good fit for testing purposes.
  However, it included a discrepancy towards the event storing solution compared to other event storage solutions.
  This issue was addressed in [#1056](https://github.com/AxonFramework/AxonFramework/issues/1056) and resolved in pull request [#1660](https://github.com/AxonFramework/AxonFramework/pull/1660).
  
* In issue [#1733](https://github.com/AxonFramework/AxonFramework/issues/1733) a confusion around the `EventUtils#asDomainEventMessage` was described.
  This reiterated the fact that this method is purely intended for internal use inside Axon Framework, which was not clear to the users.
  As such, it has now been deprecated, containing a clear statement why this method is not to be used.

## Release 4.4

### _Enhancements_

* Axon Framework can now be used in conjunction with [Spring Boot Developer Tools](https://docs.spring.io/spring-boot/docs/1.5.16.RELEASE/reference/html/using-boot-devtools.html).
  You can simply achieve this by adding the required dev-tools dependency to your project.

* As a partial solution to [#1106](https://github.com/AxonFramework/AxonFramework/issues/1106), Axon Server can now be used to schedule events.
  Building an `AxonServerEventScheduler` as the `EventScheduler` implementation as defined through the builder is sufficient to start with scheduling events through Axon Server.
  
* An `EventTrackerStatusChangeListener` can now be configured for a `TrackingEventProcessor`, as was requested in [#1338](https://github.com/AxonFramework/AxonFramework/issues/1338).
  It can be configured through the `TrackingEventProcessorConfiguration`, allowing users to react upon status changes of each thread processing event messages.

* Component specific message handler interceptors can now be defined through a dedicated annotation: the `@MessageHandlerInterceptor` annotation.
  This annotation allows you to introduce a specific bit of logic to be invoked _prior_ to entering the message handling function or after invocation.
  It for example allows the additional introduction of a `@ExceptionHandler` annotation, allowing you to specifically deal with the exceptions thrown from your message handlers.
  The original pull request can be found under [#1394](https://github.com/AxonFramework/AxonFramework/pull/1394).
  For more specifics on using this annotation, check ou the [@MessageHandlerInterceptor](../../axon-framework/messaging-concepts/message-intercepting.md#messagehandlerinterceptor) section.

* Configuring a `Snapshotter` and `SnapshotFilter` have been simplified in this release. 
  Pull request [#1447](https://github.com/AxonFramework/AxonFramework/pull/1447) shares the load of allowing for distinct `Snapshotter` configuration.
  Issue [#1391](https://github.com/AxonFramework/AxonFramework/issues/1391) describes the intent to the configuration of snapshot filtering to be performed on Aggregate level.
  The former can be configured through the `Configurer`, whereas the latter is by usage of the `AggregateConfigurer`.

### _Bug Fixes_

* The `AggregateTestFixture` was incorrectly noting an old method in one of its exceptions.
  This has been marked and resolved in [#1428](https://github.com/AxonFramework/AxonFramework/issues/1428).

* The `CommandValidator` and `EventValidator` had a minor discrepancy; namely, the `CommandValidator` cleared out contained commands upon starting whereas the `EventValidator` didn't.
  Pull request [#1438](https://github.com/AxonFramework/AxonFramework/pull/1438) resolved the problem at hand. 

For a full list of all the feature request and enhancements done for release 4.4, you can check out [this](https://github.com/AxonFramework/AxonFramework/milestone/45?closed=1) page.

## Release 4.3

### _Enhancements_

* Aggregate Polymorphism has been introduced, allowing for an aggregate hierarchy to come naturally from a domain model.
  To set this up, the `AggregateConfigurer#withSubtypes(Class... aggregates)` method can be used.
  In a Spring environment, an aggregate class hierarchy will be detected automatically.
  For more details on this feature, read up on it [here](../../axon-framework/axon-framework-commands/modeling/aggregate-polymorphism.md).

* An Axon application will now shutdown more gracefully than it did in the previous releases.
  This is achieved by marking specific methods in Axon's infrastructure components as a `@StartHandler` or `@ShutdownHandler`.
  A 'phase' is required in those, specifying when the method should be executed.
  If you want to add your own lifecycle handlers, you can either register a component with the aforementioned annotations or register the methods directly through `Configurer#onInitialize`, `Configuration#onStart` and `Configuration#onShutdown`.

* We have introduced the `@CreationPolicy` annotation which you can add to `@CommandHandler` annotated methods in your aggregate.
  Through this, it is possible to define if such a command handler should 'never', 'always' or 'create' an aggregate 'if-missing'.
  For further explanation read the [Aggregate Command Handler Creation Policy](../../axon-framework/axon-framework-commands/command-handlers.md#aggregate-command-handler-creation-policy) section.

* Both the `XStreamSerializer` and `JacksonSerializer` provide a means to toggle on "lenient serialization" through their builders.

* Various test fixture improvements have been made, such as options to register a `HandlerEnhancerDefinition`, a `ParameterResolverFactory` and a `ListenerInvocationErrorHandler`.
  Additional validations have been added too, revolving around asserting scheduled events and deadline message.
  The [Test Fixture](../../axon-framework/testing/commands-events.md) page has been updated to define these new operations accordingly.

* The `TrackingEventProcessor#processingStatus` method as of 4.3 exposes more status information.
  The current token position, token-at-reset, is-merging and merge-completed position have been added to the set.
  Read the [Event Tracker Status](../../axon-framework/monitoring/processors.md#event-tracker-status-a-idevent-tracker-statusa) section for more specifics on this.

### _Bug Fixes_

* A `ConcurrencyException` was thrown when an aggregate was created at two distinct JVM's at the same time.
  As `ConcurrencyException`s are typically retryable,  the creation command would be issued again if a `RetryScheduler` was in place.
  Retrying this operation is however useless and hence has been replaced for an `AggregateStreamCreationException` in pull request [\#1333](https://github.com/AxonFramework/AxonFramework/pull/1333).

* The test fixtures for state-stored aggregates did unintentionally not allow resource injection.
  This problem has been resolved in pull request [#1315](https://github.com/AxonFramework/AxonFramework/pull/1315).

* The `MultiStreamableMessageSource` did not deal well with one or several exceptional streams.
  Hence exception handling has been improved on this matter in [#1325](https://github.com/AxonFramework/AxonFramework/pull/1325).

For a complete list of all the changes made in 4.3 you can check out [this](https://github.com/AxonFramework/AxonFramework/milestone/42?closed=1) page.

## Release 4.2

### _Enhancements_

* Axon Framework applications can now use tags to support a level of 'location awareness' between Axon clients and Axon Server instances.
  This feature is further described [here](../../axon-server/administration/tagging.md).

* Axon Server already supported several contexts, but Axon Framework application could not specify to which context message should be dispatched.
  The Axon Server Connector has been expanded with a `TargetContextResolver` to allow just this.

* A new implementation of the `StreamablbeMessageSource` has been implemented: the `MultiStreamableMessageSource`.
  This implementation allows pairing several "streamable" message sources into a single source.
  This can in turn be used to for example read events from several distinct contexts for a single Tracking Event Processor.

* Handler Execution Exception now allow application specific information to be sent back over the wire in case of a distributed set up.

* The `TrackingToken` interface now provides an estimate of it's relative position in the event stream through the `position()` method.

* `Optional` return types can now be used for Query Handling methods.  

### _Bug Fixes_

* An Aggregate's `Snapshotter` was not auto configured when Spring Boot is being used, as was filed under [\#932](https://github.com/AxonFramework/AxonFramework/issues/932).

* The `CommandResultMessage` was returned as `null` when using the [`DisruptorCommandBus`](./).
  This was solved in pull request [\#1169](https://github.com/AxonFramework/AxonFramework/pull/1169).

* The `ScopeDescriptor` used by the `DeadlineManager` had serialization issue when a user would migrate from an Axon 3.x application to Axon 4.x.
  The `axon-legacy` package has been expanded to contain legacy `ScopeDescriptor`s to resolve this problem.

For a full list of all features, enhancements and bugs, check out the [issue tracker](https://github.com/AxonFramework/AxonFramework/milestone/38?closed=1).

## Release 4.1

### _Enhancements_

* The `TrackingEventProcessor` now has an API to split and merge `TrackingTokens` during runtime of an application.
  Axon Server has additions to the UI to split and merge a given Tracking Event Processor's tokens.

* Next to [Dropwizard](https://metrics.dropwizard.io/4.0.0/) metrics the framework now also supports [Micrometer](https://micrometer.io/) metrics.
  The `MessageMonitor` interface is used to allow integration with Micrometer.
  Lastly, we are incredibly thankful that this has been introduced as a community contribution.

* Primitive types are now supported as `@QueryHandler` return types.

* We have introduced the `EventGateway` in a similar fashion as the `CommandGateway` and `QueryGateway`.
  As with the command and query version, the `EventGateway` provides a simpler API when it comes to dispatching Events on the `EventBus`.

### _Bug Fixes_

* Command and Query message priority was not set correctly for the Axon Server Connector.
  This issue has been addressed under bug [\#1004](https://github.com/AxonFramework/AxonFramework/pull/1004).

* The `CapacityMonitor` was not registered correctly for Event Processor, which user "Sabartius" resolved under issue [\#961](https://github.com/AxonFramework/AxonFramework/issues/961).

* Some exception were not reported correctly and/or clearly when utilizing the Axon Server Connector \(issue marked under number [\#945](https://github.com/AxonFramework/AxonFramework/pull/945)\).

We refer to [this](https://github.com/AxonFramework/AxonFramework/milestone/31?closed=1) page for a full list of all the changes.

## Release 4.0

### _Enhancements_

* The package structure of Axon Framework has changed drastically with the aim to provide users the option to pick and choose.
  For example, if only the messaging components of framework are required, one can directly depend on the `axon-messaging` package.

* In part with the package restructure, all components which leverage another framework to provide something extra have been given their own repository.
  These repositories are called the [Axon Framework Extensions](https://github.com/AxonFramework?utf8=%E2%9C%93&q=extensions&type=&language=).

* The configuration of Event Processor has been replaced and greatly fine tuned with the addition of the `EventProcessingConfigurer`.

* Some new defaults have been introduced in release 4.0, like a bias towards expecting a connection with Axon Server.
  Another important chance is the switch from defaulting to Tracking Processors instead of Subscribing Processors.

* The notion of a `CommandResultMessage` has been introduced as a dedicated message towards the result of command handling.

* To simplify configuration and more easily overcome deprecation, the [Builder pattern](https://en.wikipedia.org/wiki/Builder_pattern) has been implemented for all infrastructure components.

### _Bug Fixes_

The bugs marked for release 4.0 were issues introduced to new features or enhancements. As such they should not have impacted users in any way. Regardless, the full list can be found [here](https://github.com/AxonFramework/AxonFramework/issues?utf8=%E2%9C%93&q=is%3Aclosed+milestone%3A%22Release+4.0%22++label%3A%22Type%3A+Bug%22).

For more details, check the list of issues [here](https://github.com/AxonFramework/AxonFramework/milestone/28?closed=1).
