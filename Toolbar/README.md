# Toolbar

### set you style
```xml
<!-- Base application theme. -->
<style name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar">
   <!-- Customize your theme here. -->
   ...
   <item name="windowActionBar">false</item>
   <item name="windowNoTitle">true</item>
</style>
```
### XML
```xml
<android.support.v7.widget.Toolbar xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/toolbar"
    android:layout_width="match_parent"
    android:layout_height="?attr/actionBarSize"
    android:background="@color/colorPrimary"
    app:theme="@style/Toolbar_Text_White">
</android.support.v7.widget.Toolbar>
```