# International Phone Field Package

[![Pub Version](https://img.shields.io/pub/v/flutter_intl_phone_field?color=blue&style=plastic)](https://pub.dev/packages/flutter_intl_phone_field)
[![GitHub Repo stars](https://img.shields.io/github/stars/mohesu/flutter_intl_phone_field?color=gold&style=plastic)](https://github.com/mohesu/flutter_intl_phone_field/stargazers)
[![GitHub Repo forks](https://img.shields.io/github/forks/mohesu/flutter_intl_phone_field?color=slateblue&style=plastic)](https://github.com/mohesu/flutter_intl_phone_field/fork)
[![GitHub Repo issues](https://img.shields.io/github/issues/mohesu/flutter_intl_phone_field?color=coral&style=plastic)](https://github.com/mohesu/flutter_intl_phone_field/issues)
[![GitHub Repo contributors](https://img.shields.io/github/contributors/mohesu/flutter_intl_phone_field?color=green&style=plastic)](https://github.com/mohesu/flutter_intl_phone_field/graphs/contributors)

A customized Flutter TextFormField to input international phone number along with country code.

This widget can be used to make customized text field to take phone number input for any country along with an option to choose country code from a dropdown.

## Screenshots

<img src="https://github.com/rvndsngwn/flutter_intl_phone_field/blob/master/image-1.png?raw=true" height="500px"> <img src="https://github.com/rvndsngwn/flutter_intl_phone_field/blob/master/image-2.png?raw=true" height="500px"> <img src="https://github.com/rvndsngwn/flutter_intl_phone_field/blob/master/image-3.png?raw=true" height="500px">

## Installing

To use this package:

Run this command:

```yaml
flutter pub add flutter_intl_phone_field
```

Or, add the following to your `pubspec.yaml` file:

```yaml
dependencies:
  flutter_intl_phone_field: ^<latest_version>
```

Sometimes you may want to use the latest version of the package, instead of a published version. To do that, use the `git` syntax:

```yaml
dependencies:
  flutter_intl_phone_field:
    git:
      url: git://github.com/rvndsngwn/flutter_intl_phone_field.git
      ref: master
```

## How to Use

Simply create a `IntlPhoneField` widget, and pass the required params:

```dart
IntlPhoneField(
    decoration: InputDecoration(
        labelText: 'Phone Number',
        border: OutlineInputBorder(
            borderSide: BorderSide(),
        ),
    ),
    initialCountryCode: 'IN',
    onChanged: (phone) {
        print(phone.completeNumber);
    },
)
```

Use `initialCountryCode` to set an initial Country Code.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## LICENSE

This project is licensed under the MIT license. See [LICENSE](LICENSE) for more information.
