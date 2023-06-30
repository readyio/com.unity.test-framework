# Unity Test Framework Extended

This repository is an extended version of Unity's native Test Framework package. The extensions provide support for asynchronous testing in Unity, with the addition of several new attributes.

## Features

The following async attributes have been added to support async tests:

- `AsyncOneTimeSetUp`: This attribute is used to mark a method that is called once before any of the tests in a test class have run. This can be used for async setup operations that need to be performed once per class, such as async loading of assets or any other async initialization code.
  
- `AsyncOneTimeTearDown`: This attribute is used to mark a method that is called once after all the tests in a test class have run. This can be used for async cleanup operations that need to be performed once per class, such as async disposal of resources or any other async cleanup code.

- `AsyncTest`: This attribute is used to mark a method to be used as a test. The marked method can be an async method and the testing framework will correctly wait for it to complete before marking the test as finished.

- `AsyncSetUp`: This attribute is used to mark a method that is called before each test is run. This can be used for async setup operations that need to be performed before each test, such as async initialization of test data.

- `AsyncTearDown`: This attribute is used to mark a method that is called after each test has run. This can be used for async cleanup operations that need to be performed after each test, such as async disposal of test data.

## Getting Started

To install the package, use the Unity Package Manager and follow the steps:

1. Open Unity and go to `Window -> Package Manager`.
2. Click on `+` and then `Add package from git URL...`.
3. Enter the following URL: `https://github.com/readyio/com.unity.test-framework.git#1.1.33`.
4. Click `Add`.

You need Unity version 2019.2 or later to use this package.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

Test Framework copyright © 2020 Unity Technologies ApS

Licensed under the Unity Companion License for Unity-dependent projects--see [Unity Companion License](http://www.unity3d.com/legal/licenses/Unity_Companion_License). 

Unless expressly provided otherwise, the Software under this license is made available strictly on an “AS IS” BASIS WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED. Please review the license for details on these and other terms and conditions.
