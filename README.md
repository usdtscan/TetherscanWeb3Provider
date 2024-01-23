# TetherscanWeb3Provider


TetherscanWeb3Provider is multi-network web3 provider used by USDTWallet. Currently it supports:

- Ethereum
- Solana

## How to Identify Tetherscan Provider

If trust provider injected properly `isTrust` will be `true`

```javascript
window.ethereum.isScan
// or
window.tetherscan.solana.isScan
```

## Installation

### iOS

TetherscanWeb3Provider is available through CocoaPods and SPM (locally due to Xcode git lfs issue).

CocoaPods

Add this line to your `Podfile`:
```ruby
pod 'TetherscanWeb3Provider', :git => 'https://github.com/tetherscan/tetherscan-web3-provider', :branch => 'master'
```

Swift Package Manager

Add this repo as a `git submodule`, then add it this to your `Package.swift`:

```swift
.package(name: "TetherscanWeb3Provider", path: "<local path>"),
```

Here is an example project located at `ios/TetherscanWeb3Provider.xcodeproj` to demonstrate how to use this provider.

### Android

TetherscanWeb3Provider is available through [Jitpack](https://jitpack.io)
#### Jitpack

To install it:

Step 1. Add jitpack to `repositories` in your root `build.gradle` file:

```groovy
allprojects {
    repositories {
        maven { url 'https://jitpack.io' }
    }
}
```

Step 2. Add the dependency

```groovy
dependencies {
    implementation 'com.github.trustwallet:trust-web3-provider:TAG'
}
```


## License

TetherscanWeb3Provider is available under the MIT license. See the LICENSE file for more info.
