# Toolbar

#### set you style in style.xml
```xml
<!-- Base application theme. -->
<style name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar">
   <!-- Customize your theme here. -->
   ...
   <item name="windowActionBar">false</item>
   <item name="windowNoTitle">true</item>
</style>
```
#### create toolbar.xml
```xml
<?xml version="1.0" encoding="utf-8"?>
<android.support.v7.widget.Toolbar xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/toolbar"
    android:layout_width="match_parent"
    android:layout_height="?attr/actionBarSize"
    android:background="@color/colorPrimary"
    app:theme="@style/Toolbar_Color">
</android.support.v7.widget.Toolbar>
```
#### Example style toolbar
```xml
 <!--For color toolbar may be multi color-->
<style name="Toolbar_Color">
   <item name="android:textColorSecondary">@color/White_Text_Primary</item>
   <item name="titleTextColor">@color/White_Text_Primary</item>
</style>
```
