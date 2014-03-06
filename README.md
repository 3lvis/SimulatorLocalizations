Switching Localizations in iOS is a hassle, doing the **Settings -> General -> International -> Choose Language** dance is anything but fun.

Luckily for us Xcode provides a great way to switch between Languages easily.

![Alternative schemes](https://coderwall-assets-0.s3.amazonaws.com/uploads/picture/file/2691/Screen_Shot_2014-03-06_at_10.06.53.png)

All you have to do is duplicate your Scheme and add these arguments.

For the language:

    -AppleLanguages (fr)

For the region (time, currency and others):

    -AppleLocale fr_FR

And as a BONUS, you can tell Xcode to WARN YOU if you don't have localized strings, this will appear in your Console and they will be UPPERCASE in the app:

    -NSShowNonLocalizatedStrings YES

![Arguments](https://coderwall-assets-0.s3.amazonaws.com/uploads/picture/file/2692/Screen_Shot_2014-03-06_at_10.07.19.png)
