# AdMobCompose
This repositry contains code to implement Google Ad Mob in compose. 


# Steps:
- Adding Implementation In App Level Gradle
  ```kotlin
  implementation 'com.google.android.gms:play-services-ads:22.0.0'

- Implementing Class in Android
  ```kotlin
  class MainActivity : ComponentActivity() {
    @OptIn(ExperimentalMaterial3Api::class)
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        MobileAds.initialize(this) {}
        MobileAds.setRequestConfiguration(
          RequestConfiguration.Builder().setTestDeviceIds(listOf("ABCDEF012345")).build()
        )
  }

  - Implementing Funtion
  

