Bordered-Textview
=====

Download
--------
Use Gradle:

```gradle
repositories {
  google()
  mavenCentral()
}

dependencies {
  implementation 'com.github.gbhargavv:Bordered-Textview:1.0'
}
```

Or Maven:

```xml
<dependency>
    <groupId>com.github.gbhargavv</groupId>
    <artifactId>Bordered-Textview</artifactId>
    <version>Tag</version>
</dependency>
```

Simple use cases will look something like this:

```java
// For a simple view:
@Override public void onCreate(Bundle savedInstanceState) {
    
    BorderedTextView borderedTextView = findViewById(R.id.txt);
    // Customize using below code
    borderedTextView.setBorderedColor(Color.GREEN);
    borderedTextView.setIncludeFontPadding(false);
    borderedTextView.setLineSpacing(0f, 0f);
    borderedTextView.setBorderTypeface(Typeface.createFromAsset(getAssets(), "Mont-Bold.ttf"));
    borderedTextView.setBorderWidth(3);
    borderedTextView.setInsetColor(Color.BLACK);
    borderedTextView.setTextSizes(30);
}
```

```xml
 <BorderedTextView
    android:id="@+id/txt"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:text="@string/app_name" />
```

